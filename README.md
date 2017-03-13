<h2>
imageViewBrowser
图片浏览/查看器
</h2>
<hr> 
<h3>
<span color="red">描述:</span>一种图片浏览器,支持查看大图,缩放,SD_WebImage下载,进度条,长按保存到相册,<br>
支持url数组,字符串链接数组,二进制数组的多功能图片查看器<br>
</h3>
<hr> 
<h4>
使用方法:<br>
 1.将文件夹导入项目<br>
 2.#import "JZAlbumViewController.h"<br>
 3.button点击事件<br>
<pre><code>
#pragma mark - 查看大图<br>
- (void)p_btnClickCheckBigImage:(UIButton *)btn {//点击事件
    JZAlbumViewController *jzAlbumVC = [[JZAlbumViewController alloc]init];
    jzAlbumVC.currentIndex = btn.tag; //当前点击图片的索引
    //webImageUrl可以为url数组, 可以为urlString 数组, 可以为二进制 UIImage 数组
    jzAlbumVC.imgArr = [NSMutableArray arrayWithArray:webImageUrl];
    [self presentViewController:jzAlbumVC animated:YES completion:nil];
}
</code></pre>
</h4>
<hr> 
<div>
<img src="./img1" alt="Smiley face" ><br>
<img src="./img2" alt="Smiley face" ><br>
</div>
<hr> 
<h3>
1.改写自//jinzelu  Copyright (c) 2015年 jinzelu. All rights reserved.<br>
2.本人增加了图片保存到相册,支持UIImage数据,修改了偶尔crash的 bug!<br>
</h3>

