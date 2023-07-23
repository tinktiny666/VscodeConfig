# VscodeConfig
vscode配置详解
## 配置

然后进入VSCode,点击Open Folder或者点击左上角File -> Open Folder，然后打开刚刚建的文件夹，选择信任父级文件夹

点击这个图标新建一个文件夹，命名为.vscode（注意必须是这个名字！）

在.vscode文件下建立四个文件

//c_cpp_properties.json
//launch.json
//settings.json
//tasks.json


# 首先是c_cpp_properties.json



注意compilerPath这一项要把路径改成刚才g++的安装路径：找到刚刚的安装文件夹->MinGW->bin->g++,exe ,然后复制或者手动把g++.exe的路径敲上去，格式要跟上面代码段一样

# 然后是launch.json



## c/c++编写格式设置-函数右侧大括号换行，其他不换行

打开设置找到 "C_Cpp: Clang_format_style" 这项，填入以下代码：

{ BasedOnStyle: LLVM, UseTab: Never, IndentWidth: 4, TabWidth: 4, BreakBeforeBraces: Linux, AllowShortIfStatementsOnASingleLine: false, IndentCaseLabels: false, ColumnLimit: 0, AccessModifierOffset: -4, NamespaceIndentation: All, FixNamespaceComments: false }

