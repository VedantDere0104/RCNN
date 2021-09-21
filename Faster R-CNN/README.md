# Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks :- 

Pytorch Implementation of Faster RCNN .

## Abstract :- 
State-of-the-art object detection networks depend on region proposal algorithms to hypothesize object locations.
Advances like SPPnet [1] and Fast R-CNN [2] have reduced the running time of these detection networks, exposing region
proposal computation as a bottleneck. In this work, we introduce a Region Proposal Network (RPN) that shares full-image
convolutional features with the detection network, thus enabling nearly cost-free region proposals. An RPN is a fully convolutional
network that simultaneously predicts object bounds and objectness scores at each position. The RPN is trained end-to-end to
generate high-quality region proposals, which are used by Fast R-CNN for detection. We further merge RPN and Fast R-CNN
into a single network by sharing their convolutional features—using the recently popular terminology of neural networks with
“attention” mechanisms, the RPN component tells the unified network where to look. For the very deep VGG-16 model [3],
our detection system has a frame rate of 5fps (including all steps) on a GPU, while achieving state-of-the-art object detection
accuracy on PASCAL VOC 2007, 2012, and MS COCO datasets with only 300 proposals per image. In ILSVRC and COCO
2015 competitions, Faster R-CNN and RPN are the foundations of the 1st-place winning entries in several tracks.


## Architecture :- 
![image](https://user-images.githubusercontent.com/76057253/134172582-8db9edee-461e-4746-8e0c-0f1d59ca4043.png)


## Results :- 
![image](https://user-images.githubusercontent.com/76057253/134172675-e55c3e72-e1fb-4a64-a81a-0ac06384f22b.png)

```
@misc{ren2016faster,
      title={Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks}, 
      author={Shaoqing Ren and Kaiming He and Ross Girshick and Jian Sun},
      year={2016},
      eprint={1506.01497},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
