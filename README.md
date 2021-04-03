# Kaggle-HuBMAP-Hacking-the-Kidney
Kaggle-HuBMAP-Hacking-the-Kidney



## End Date (Final Submission Deadline): 
February 1 , 2021 11:59 PM UTC] 11:59 PM UTC

### Selected teams present their solutions to Judges:
February 5, 2021

### Winners announced 
February 12, 2021

### Goal
Your challenge is to detect functional tissue units (FTUs) across different tissue preparation pipelines. 

An FTU is defined as a “three-dimensional block of cells centered around a capillary, such that each cell in this block is within diffusion distance from any other cell in the same block”. 

The goal of this competition is the implementation of a successful and robust glomeruli FTU detector.

-------

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
     Y_SHFT = -44      LB     ver



X_SHFT = -24


