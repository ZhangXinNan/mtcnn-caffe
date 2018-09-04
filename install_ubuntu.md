conda install opencv
conda install scikit-image

## 1 google.protobuf
```
Failed to include caffe_pb2, things might go wrong!
Traceback (most recent call last):
  File "test_zx.py", line 5, in <module>
    import caffe
  File "/home/zhangxin/github/caffe/python/caffe/__init__.py", line 4, in <module>
    from .proto.caffe_pb2 import TRAIN, TEST
  File "/home/zhangxin/github/caffe/python/caffe/proto/caffe_pb2.py", line 6, in <module>
    from google.protobuf.internal import enum_type_wrapper
ModuleNotFoundError: No module named 'google'
```


```
conda install protobuf
```


## 2 
```
Traceback (most recent call last):
  File "test_zx.py", line 109, in <module>
    main(get_args())
  File "test_zx.py", line 96, in main
    rectangles = detectFace(imgpath,threshold)
  File "test_zx.py", line 27, in detectFace
    caffe_img = (img.copy()-127.5)/128
AttributeError: 'NoneType' object has no attribute 'copy'
```

img is None
