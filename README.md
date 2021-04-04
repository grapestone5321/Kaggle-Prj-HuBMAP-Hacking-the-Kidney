# Kaggle-HuBMAP-Hacking-the-Kidney
Kaggle-HuBMAP-Hacking-the-Kidney

-------

## Submission Deadline

### End Date (Final Submission Deadline): 
May 10, 2021 at 11:59 PM UTC] 11:59 PM UTC

### Selected teams present their solutions to Judges:
May 17, 2021

### Winners announced 
May 21, 2021


-------

## Task

Your challenge is to detect functional tissue units (FTUs) across different tissue preparation pipelines. 

An FTU is defined as a “three-dimensional block of cells centered around a capillary, such that each cell in this block is within diffusion distance from any other cell in the same block”. 

The goal of this competition is the implementation of a successful and robust glomeruli FTU detector.

-------

## Evaluation

This competition is evaluated on the mean Dice coefficient. 

The Dice coefficient can be used to compare the pixel-wise agreement between a predicted segmentation and its corresponding ground truth. 

The Dice coefficient is defined to be 1 when both X and Y are empty. 

The leaderboard score is the mean of the Dice coefficients for each image in the test set.

### Dice coefficient
https://en.wikipedia.org/wiki/S%C3%B8rensen%E2%80%93Dice_coefficie

-------

## Welcome to the HuBMAP: Hacking the Kidney Competition! by Leah Scherschel

To help you get started, please check out the following notebooks:

Dataset Details https://www.kaggle.com/leahscherschel/dataset-details
(Background Information and Specifications of the Dataset)

Glomeruli Detection Related Works https://www.kaggle.com/leahscherschel/glomeruli-detection-related-works
(Prior Work on Glomeruli Detections in Microscopy Images)

Polygon to Pixel Mask Conversion https://www.kaggle.com/leahscherschel/polygon-to-pixel-mask-conversion
(How to Convert Polygon Masks to Pixel Masks)

Run-Length Encoding https://www.kaggle.com/leahscherschel/run-length-encoding
(How to Perform Run-Length Encoding)

-------

## Dataset

- efficientnet_1_0_0: Vasiliy updated 4 months ago (Version 1)


-------

## Progress

### Public Best LB Score: 0.918

### Private Score: 






-------

## Global Mask Shift 
https://www.kaggle.com/frankx7/global-mask-shift

### Public Score: 0.866


-------


## Global Mask Shift
https://www.kaggle.com/frankx7/global-mask-shift

      Public Score: 0.866
### dfpred

x_shift = -21, y_shift = -43: 

      dfpred = pd.read_csv('../input/best-public-hubmap/submission_public_TPU.csv')
      dfpred = pd.read_csv('../input/hubmap-lb0849/submission_subm_V14_TPU.csv')        LB 0.866    ver5
      dfpred = pd.read_csv('../input/hubmaplb0850/submission_LB0.850.csv')              LB 0.867    ver6
      dfpred = pd.read_csv('/kaggle/input/hubmap865/hubmap-865.csv')                    LB 0.846    ver7
      
dfpred = pd.read_csv('../input/hubmaplb0850/submission_LB0.850.csv'):

x_shift = -21:

      y_shift = -43                LB 0.867    ver6
      y_shift = -42                LB 0.867    ver8                123 -> 100
      y_shift = -41                LB 0.867    ver9                100 -> 100

y_shift = -42:

      x_shift = -21                LB 0.867    ver8      
      x_shift = -20                LB 0.867    ver10              100 -> 96
      x_shift = -19                LB 0.867    ver11               97 -> 94
      x_shift = -18                LB 0.867    ver12   --- Best    94 -> 93
      x_shift = -17                LB 0.867    ver13               93 -> 93
      
 
x_shift = -18, y_shift = -42: 
 
      dfpred = pd.read_csv('../input/best-public-hubmap/submission_public_TPU.csv')     LB 0.866    ver14
      dfpred = pd.read_csv('../input/hubmap-lb0849/submission_subm_V14_TPU.csv')        LB 0.866    ver15
      dfpred = pd.read_csv('../input/hubmaplb0850/submission_LB0.850.csv')              LB 0.867    ver12 
      dfpred = pd.read_csv('/kaggle/input/hubfastai836/hub-fast-ai-836.csv')            LB 0.853    ver16
 
-------      
      
## HuBMAP fast.ai starter sub
https://www.kaggle.com/iafoss/hubmap-pytorch-fast-ai-starter-sub


### bs = 64

      bs = 16      LB 0.836    ver3, 4
      bs = 32      LB 0.836    ver2
      bs = 64      LB 0.836    ver1

### self.drop_aspp = nn.Dropout2d(0.5):

bs = 64:

      self.drop_aspp = nn.Dropout2d(0.5)    LB 0.836    ver1
      self.drop_aspp = nn.Dropout2d(0.8)    LB 0.836    ver5


-------

## HuBMAP - Hacking the Kidney


### Y_SHFT default = -40

X_SHFT = -24:

     Y_SHFT = -40      LB 0.916    ver1
     Y_SHFT = -44      LB 0.916    ver2    --- Best    206 -> 205



X_SHFT = -24

-------

## Kidney Unet model (keras) inference
https://www.kaggle.com/vgarshin/kidney-unet-model-keras-inference

      Public Score 0.918       ver33    --- Best


-------
