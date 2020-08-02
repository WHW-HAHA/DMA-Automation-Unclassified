# Introduction
Dynamic mooring analysis(DMA) is one of the most important businesses in Royal HaskoningDHV maritime department.

<br>The DMA automation overall aims at automating the DMA workflow in Royal HaskoningDHV, and enabling faster delivery of DMA projects, increasing quality of works and the interaction with other offices and initiatives. The whole DMA automation contains the development of local automated packages, cloud computing and cloud storage.  

<br>All the scripts folders in each working folder are empty, but the input and output are given in the input and output folder. As a visitor, please regard those scripts folders as black boxes.

<br>The purpose of this repository is to outline the structure of this project and showcase the output of a few commonly used modules.

## Illustration of the work flow
![Illustration](https://user-images.githubusercontent.com/43483189/88797943-67878d80-d1a4-11ea-803b-ec9887f1007f.png)
## Languages:
- Python 
- SQL
- Lua
## Platform:
- Deployment: Microsoft Azure
- Development and Maintenance: Microsoft Azure Devops
- Django

# Typical steps of using this automated platform
## Preparations for doing a DMA project**
- Step 0. Read look up note and manual about using DMA automation platform
  ![Illustration](https://user-images.githubusercontent.com/43483189/88807581-30b87400-d1b2-11ea-8469-0709fe1b3e73.png) 
  *Look up note*
  
- Step 1. Model build up 
  - Prepare the numerical model in Excel
  ![Illustration](https://user-images.githubusercontent.com/43483189/88803822-52632c80-d1ad-11ea-80a7-3a31a23b6c8f.png)  
  *A typical numerical model in Excel*
  
  - Transform the Excel model to a numerical model(xml format), which can be understood by numerical modelling software aNySIM
  [.xml Template](/Preparations for doing a DMA project/Outputs/Template.xmf)
 
  - Execute the visualize the numerical model and do test runs to check the correctness of the numeric model
  
  *The visualization of the numerical model*
  
- Step 2. Create a batch of simulations
  - Create a matrix of combination of environmental conditions
  ![Illustration](https://user-images.githubusercontent.com/43483189/89121111-4f718000-d4bc-11ea-8f49-8e0ccbf9778c.png)  
  *A typical matrix of a combination of a environmental conditions*
  
  - Create a batch of simulations according to the matrix of environmental conditions
  [Folder of a batch of simulations](/Execute the runs of DMA project/Xmf_Template_to_Batch/Outputs)  
  *A batch of runs for various of environmental conditions*

## Execute the runs of DMA simulation
- Step 3. Upload the simulations to DMA portal to run the simulations and compress the output of all runs into a csv file.
  
  ![Interface](https://user-images.githubusercontent.com/43483189/88804194-db7a6380-d1ad-11ea-9e7d-b59f72551afe.png)
  *Interface to upload the runs to initiate a new project and execute cloud computing*
  
- Step 4. Export the output to local work space to post process the result.

  ![Interface](https://user-images.githubusercontent.com/43483189/88804429-2c8a5780-d1ae-11ea-9025-dea671b37a94.png)
  *Interface to download the output*
  
## Post process the output data
- Step 5. Data analysis 

# Showcase of a series of typical data analysis 
- Typical bar plot

  ![Bar plots](https://user-images.githubusercontent.com/43483189/88808140-c81dc700-d1b2-11ea-9b31-e91a05be3649.png)
- Typical interactive polar plot

  ![Interactive polar plot](https://user-images.githubusercontent.com/43483189/88808221-dec41e00-d1b2-11ea-8233-9dc1f7111e28.png)
- Typical time signal analysis

  ![Time signals](https://user-images.githubusercontent.com/43483189/88809444-70805b00-d1b4-11ea-9e06-7dfc508ac82a.png)
- Typical statical data analysis

  ![Statistics](https://user-images.githubusercontent.com/43483189/88808610-6742be80-d1b3-11ea-9b3d-768367fdfb54.jpg)
- Typical scatter plot with the probability of occurrence

  ![Scatter](https://user-images.githubusercontent.com/43483189/88809173-18495900-d1b4-11ea-93c0-3b4e689ca6e1.png)






