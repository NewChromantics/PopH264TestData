Some (troublesome?) H264 data streams which SHOULD decode.

Extracting HEVC annexb bitstream from mp4
----------
- `ffmpeg -i ./AppleSpatialRobotNutcracker.mov -c:v copy -bsf hevc_mp4toannexb ./AppleSpatialRobotNutcracker.h265`


Extracting H264 annexb bitstream from mp4
----------
- `AppleSpatialRobotNutcracker.mov` is hevc, so convert to h264
- `ffmpeg -i ./AppleSpatialRobotNutcracker.mov ./AppleSpatialRobotNutcracker.mp4`
- `ffmpeg -i ./AppleSpatialRobotNutcracker.mp4  -c:v copy -bsf h264_mp4toannexb ./AppleSpatialRobotNutcracker.h264`
