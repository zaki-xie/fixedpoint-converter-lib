# fixedpoint-converter-lib
浮点转定点算法纯C语言实现的函数库存档，包含fr_math库与IQmath库
# 库开源地址
fr_math(https://github.com/deftio/fr_math)  
IQmath(https://github.com/mikisama/IQmath)

# 背景
出于嵌入式项目的需求，要在一块超低成本的芯片上运行浮点运算，为优化性能，最终选择了上述两个库，上述库具有如下的几点优势：  
1、纯C语言实现的开源代码（TI的IQmath有专门针对TI平台芯片的优化，但仍支持纯C语言的移植），可轻松移植多平台运行；  
2、按位缩放实现的浮点数与定点数转换，简单测试了一下乘法，两库的精度是相同的；  
3、fr_math提供了函数封装和底层define方式定义的算法两种使用方式，IQmath提供了更丰富的函数封装调用方式。如果追求极致性能，调用fr_math的底层函数理论上更加高效，但是需要注意自己手动进行缩放，防止运算结果错误。

# 如何使用
请参考我的[博客文章](https://blog.csdn.net/qq_46314975/article/details/155517395?sharetype=blogdetail&sharerId=155517395&sharerefer=PC&sharesource=qq_46314975&spm=1011.2480.3001.8118)。

如果该项目对您有所帮助，请帮我和开源库作者们点个星星，若您有任何疑问，可在本项目或我的博客（博客回复可能更快）中提出，我会尽力为您解答。
