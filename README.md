# mokuyu-qrcode
## 生成二维码
下面给二维码添加logo的功能
```
/**
 * 生成二维码图片
 * @param  integer $size    二维码大小
 * @param  string  $content 二维码内容
 * @param  string  $logo    二维码logo图片，有则加
 * @param  string  $savePath 二维码保存路径路径有效则自动保存,设置 '' 话直接输出,设置为null，则返回图像资源
 * @return [type]           [description]
 */
\ank\QRcode::build($content = '', $size = 100, $logo = '', $savePath = '')

$config = [
    // 二维码内容
    'content'              => 'test',
    // 生成图片大小
    'size'                 => 300,
    // 二维码边距
    'margin'               => 2,
    // 像素点大小
    'matrixPointSize'      => 10,
    // 容错等级 容错级别L(7%)M(15%)Q(25%)H(30%)
    'errorCorrectionLevel' => 'H',
    // 背景色
    'back_color'           => 0xFFFFFF,
    // 前景色
    'fore_color'           => 0x000000,
    // 二维码logo图片，有则加
    'logoPath'             => '',
    // 二维码保存路径路径有效则自动保存,设置 '' 话直接输出,设置为null，则返回图像资源
    'savePath'             => '',
];
\ank\QRcode::greate($config);
```