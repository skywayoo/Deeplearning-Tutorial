# Create ImageIterator

How to use own images to dataiter

1. change direction`cd mxnet/tools/`

2. create .lst file `python im2rec.py --list=True --recursive=True [list_file] [filepath] ` 

3. create .rec file `python im2rec.py --resize=256 --quality=90 --num-thread=4 [list_file] [filepath]`    

### mx.io.ImageRecordIter()

`train = mx.io.ImageRecordIter(
  path.imglist =  [list_file],
  path.imgrec     = [rec.file],
  batch.size      = 2,
  data.shape      = c(256,256,3)
)`

### mx.io.extract()

extract the iterator data

* data = `mx.io.extract(data_iter)[1]`

* labels = `mx.io.extract(data_iter)[2]`
