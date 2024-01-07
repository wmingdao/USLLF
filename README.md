# The Text Dataset for USLLF
This repo is a text dataset for Modeling the Skeleton-Language Uncertainty for 3D Action Recognition (USLLF). The paper has been submitted to IEEE Transactions on Multimedia.

This dataset is designed to describe the execution process of human actions including 1200 samples in 60 action classes, which is divided into two types: (1) global description (10 .txt files, 600 samples) and (2) part description (10 .txt files, 600 samples). The length of each sample does not exceed 90 words. Note that the action categories described in this dataset match those of **[NTU 60](https://openaccess.thecvf.com/content_cvpr_2016/papers/Shahroudy_NTU_RGBD_A_CVPR_2016_paper.pdf)**.

## How to Construct this Dataset

### Global Description
**Template/Prompt:** It is a request to describe the human action "[action]" from various body parts' views: head, hand, arm, hip, leg, and foot. Each part's description is no more than 15 words.

### Part Description
**Template/Prompt:** It is a request to describe how the human action “[action]” is performed from a global view. Note that this description is no more than 90 words.

### Generating Action Descriptions
The Templates/Prompts are fed to **[ChatGPT 4.0](https://chat.openai.com/)** as a request to generate the action descriptions by replacing the keywords "[action]" with action categories. To increase sample diversity, the request is sent for each category 10 times. 


