# UIImageView-HGCWebImage

SDWebImage 的封装，提供较方便的接口给 UIImageView，支持图片拉伸适应和高效的圆角效果。
依赖：SDWebImage, NYXImagesKit

示例代码：
```
NSString *urlstring = @"http://assets.saigao.4566.com/2016/9/10/upload_0ea5addf49e7b7ef293aa0b74468a5c1.jpg";
UIImage *loadfailImg = [UIImage imageNamed:@"loadfail"];
[_imgview hgc_setImageWithURLString:urlstring
                   placeholderImage:loadfailImg
                      loadFailImage:loadfailImg
                    scaleToFillSize:CGSizeMake(240, 128)
                    roundingCorners:HGCRectCornerAll
                        cornerRadii:8];
```
