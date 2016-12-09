# FONTSIZE
1. 字体图标属性
   <pre>
     <code>
       @font-face{
         font-family:"字体名字";
         src:url("字体路径");
       }
     </code>
   </pre>
2. 使用方式一
   
   利用unicode编码引用
   <pre>
   <code>
    @font-face {
    font-family: "字体名字";
    src: url('字体路径');
    src: url('font/iconfont.eot?#iefix') format('embedded-opentype'),
    url('font/iconfont.woff') format('woff'),
    url('font/iconfont.ttf') format('truetype'),
    url('font/iconfont.svg#iconfont') format('svg');
    }
    div{
    font-family:abc
    }  
    </code>
    <div>
    对应的unicode编码
    </div>
</pre>
    
   
3.  使用方式二
    利用类名去调用
    <pre>
         <code>
              /* css */
               @font-face {
                          font-family: "字体名字";
                          src: url('字体路径');
                          src: url('font/iconfont.eot?#iefix') format('embedded-opentype'),
                          url('font/iconfont.woff') format('woff'),
                          url('font/iconfont.ttf') format('truetype'),
                          url('font/iconfont.svg#iconfont') format('svg');
                      }
                 .iconfont{
                             font-family: abc;
                         }
                         .bike:before{
                             content: "对应的编码";
                         }    
                      
          </code>
              <div class="iconfont bike">
                 
              </div>
         
</pre>
   
   