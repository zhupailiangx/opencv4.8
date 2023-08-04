## OpenCV: Open Source Computer Vision Library

### 关闭perf Disable和调整perf failed 
### 编译
```
perf_test_data/cv/optflow/rubberwhale1.png 改成RubberWhale1.png
cd opencv4.8
mkdir build
cd build
cmake ..
make -j8 opencv_perf_core opencv_perf_imgproc
```
#### 测试结果到xlsx
```
cd perf_test_data
python3 ../modules/ts/misc/run.py ../build -t core
python3 ../modules/ts/misc/report.py core.xml -o html ->core.xlsx
```

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
