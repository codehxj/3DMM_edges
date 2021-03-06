# 3DMM_edges
This is a Matlab implementation of an algorithm for fully automatically fitting a 3D Morphable Model to a single image using landmarks and edge features. This repository is extended version of [3DMM_edges](https://github.com/waps101/3DMM_edges)


## References

[the following paper](http://arxiv.org/abs/1602.01125) ([DOI](http://dx.doi.org/10.1007/978-3-319-54427-4_28)):

A. Bas, W.A.P. Smith, T. Bolkart and S. Wuhrer. "Fitting a 3D Morphable Model to Edges: A Comparison Between Hard and Soft Correspondences". In Proc. ACCV Workshop on Facial Informatics, LNCS vol. 10117, pp. 377-391, 2016.

and (for the landmark detector):

X. Zhu and D. Ramanan. "Face detection, pose estimation and landmark localization in the wild" in Proceedings of IEEE Conference on Computer Vision and Pattern Recognition (CVPR), 2012.

## Dependencies

In order to use this code, you need to provide your own 3D Morphable Model. One such model (and the one we used while developing the code) is the [Basel Face Model](http://faces.cs.unibas.ch/bfm/?nav=1-0&id=basel_face_model). This model is freely available upon signing a license agreement. If you use the Basel Face Model, then all you need to do is set the base path to your model in the demo.m file:

Download 01_MorphableModel.mat using https://drive.google.com/open?id=1uZwxn9jP8-GwBcwpjn6nGRrk60D90_da 

```matlab
BFMbasedir = '...'; % Set this to your Basel Face Model base directory
```


## Third party licenses

This repository ships with a copy of the [Zhu and Ramanan facial feature detector](https://www.ics.uci.edu/~xzhu/face/), which was released under the following license:

> Copyright (C) 2012 Xiangxin Zhu, Deva Ramanan
> 
> Permission is hereby granted, free of charge, to any person obtaining
> a copy of this software and associated documentation files (the
> "Software"), to deal in the Software without restriction, including
> without limitation the rights to use, copy, modify, merge, publish,
> distribute, sublicense, and/or sell copies of the Software, and to
> permit persons to whom the Software is furnished to do so, subject to
> the following conditions:
>
> The above copyright notice and this permission notice shall be
> included in all copies or substantial portions of the Software.
>
> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
> EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
> MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
> NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
> LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
> OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
> WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
