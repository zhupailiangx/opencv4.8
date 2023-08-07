## OpenCV perf
关闭perf Disable,解决perf failed,调整samples=100,outliers=0
### Imgproc failed 原因
![image](https://github.com/zhupailiangx/opencv4.8/assets/120553507/c0f82035-3282-4f3b-8a52-74270046e334)


### 编译
```
cd opencv4.8
mkdir build
cd build
cmake ..
make  opencv_perf_core opencv_perf_imgproc
```
#### 测试结果到xlsx
```
cd perf_test_data
python3 ../modules/ts/misc/run.py ../build -t core
python3 ../modules/ts/misc/report.py core.xml -o html ->core.xlsx
```
---
---
## OpenCV: Open Source Computer Vision Library
### Resources

* Homepage: <https://opencv.org>
  * Courses: <https://opencv.org/courses>
* Docs: <https://docs.opencv.org/4.x/>
* Q&A forum: <https://forum.opencv.org>
  * previous forum (read only): <http://answers.opencv.org>
* Issue tracking: <https://github.com/opencv/opencv/issues>
* Additional OpenCV functionality: <https://github.com/opencv/opencv_contrib> 


### Contributing

Please read the [contribution guidelines](https://github.com/opencv/opencv/wiki/How_to_contribute) before starting work on a pull request.

#### Summary of the guidelines:

* One pull request per issue;
* Choose the right base branch;
* Include tests and documentation;
* Clean up "oops" commits before submitting;
* Follow the [coding style guide](https://github.com/opencv/opencv/wiki/Coding_Style_Guide).
