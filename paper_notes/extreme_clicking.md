# [Extreme clicking for efficient object annotation](https://arxiv.org/abs/1708.02750)

_December 2019_

tl;dr: Annotate extreme points to replace conventional bbox annotation leads to same accuracy, reduced annotation time and additional information.

#### Overall impression
This paper inspired [ExtremeNet](extremenet.md). 

#### Key ideas
- Conventional bbox annotation involves clicking on imaginary corners of a right box around the object. This is difficult as these corners are often outside the actual object and several adjustments are required to obtain a tight box.
- Annotation by extreme point clicking is only **7s per box, 5x faster** than the traditional way of drawing bbox.

#### Technical details
- Two ways to obtain annotation: "annotation party" vs crowdsourcing. The former is too costly and crowdsourcing is essential for creating large datasets.
- The bbox annotator need to pay attention to extreme points anyway to ensure accurate annotation. Clicking the top-left corner couples the localization and aligning hairlines of of top and left-most extreme point at the same time.

#### Notes
- This is promising to help annotating on distorted and undistorted image simultaneously.
- Can we train a patch-based segmentation model to help with this task?
