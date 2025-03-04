# video2screenshot

video2screenshot 是一个便捷的命令行工具，用于自动生成视频文件的多帧截图预览文件。它能帮助你快速创建视频缩略图，方便视频内容概览、管理与归档，同时也可以轻松集成到更复杂的自动化工作流中，提升视频处理效率，适合视频库整理和媒体资源管理。

## 主要特性

* 多平台支持：兼容 macOS、Linux 等可运行ffmpeg与ImageMagick的系统。
* 依赖：借助 ffmpeg 快速提取视频帧，并利用 ImageMagick 进行图像合成。
* 自动判断截图数量：根据视频长度自动化判断所需截图的数量，用户可根据注释自行修改参数以自定义规则。

## 使用方式
1. 前置条件：安装ffmpeg与ImageMagick
  * Linux：可使用`apt`命令从系统软件仓库中安装。
  * MacOS：建议先安装“Homebrew”，借助“Homebrew”安装ffmpeg与ImageMagick。
2. 从任意目录运行该脚本，该脚本接受视频文件的绝对路径作为唯一参数。运行命令举例如下：
 ```
 <path>/video2screenshots_正式版.sh "<path>/<videoFileName>.mkv"
 ```
3. 脚本所在目录下将会生成视频文件的同名文件夹，以存储临时截图文件，运行完成后会删除临时文件及文件夹。最终合成的多帧截图预览文件将会在视频所在目录下生成，与视频文件同名。

## 使用方式

1. **前置条件**  
   确保已安装以下工具：  
   - **ffmpeg**  
   - **ImageMagick**  
   - **安装方法：**  
     - **Linux：** 使用 `apt` 命令从系统软件仓库中安装。  
     - **macOS：** 推荐先安装 [Homebrew](https://brew.sh/)，然后通过 Homebrew 安装 ffmpeg 与 ImageMagick。  

2. **运行脚本**  
   在任意目录下运行该脚本，需传入视频文件的绝对路径作为唯一参数。示例命令如下：  
   ```bash
   <path>/video2screenshots.sh "<path>/<videoFileName>.mkv"
   ```
	
 3.	生成预览图
  * 脚本会在其所在目录下创建一个以视频文件同名的文件夹，用于存储临时截图文件。
  * 运行完成后，该临时文件夹及其中所有文件会被自动删除。
  * 最终生成的多帧截图预览文件将保存在视频文件所在目录中，文件名与视频文件相同。


 
