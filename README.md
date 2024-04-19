# Significance Analysis of Normalized Indices in Land Use and Land Class Classification in an Urban Landscape Using Google Earth Engine and Machine Learning

<p><i>The repository contains the code and output of the study "Significance Analysis of Normalized Indices in Land Use and Land Class Classification in an Urban Landscape Using Google Earth Engine and Machine Learning".</i></p>
<br> 
 
 ## 1. About the Study
<p>The study applies 3 ML/DL algorithms (Support Vector Machine, Random Forest, and Artificial Neural Network) to do 7 class Land Use Land Cover classification for the area of Phnom Penh in Cambodia.
The classes are- 
0 'Tree',
1 'RoadsAndPavements',
2 'SavannahGrassland',
3 'Building',
4 'Water', 
5 'AgriculturalLand', 
6 'BareLand'
</p>
<p>The algorithms are applied in 2 different combinations of Sentinel 2B dataset. One with only Bands 1, 2, 3, 4, 5, 6, 7, 8, 8A, 9, 11 and 12 of Sentinel dataset. The another contains these bands along with 4 additional bands namely, Normalized Difference Builtup Index(NDBI), Normalized Difference Vegetation Index(NDVI), Normalized Difference Water Index(NDWI), and Bare Soil Index(BSI).</p> 
<p>The objectives of this study includes understanding the impact of these indices on LULC classification, producing updated LULC maps. At the end, a new approach (hybrid) combining the outputs from the best models for each of the classes were proposed. This new approach shows the better accuracy then all other models attempted in the study.</p> 

## 2. Study Area
![image](https://github.com/KaziJahidurRahaman/indices-significance/blob/main/Maps/study_area_.png)


## 3. General Workflow
![image](https://github.com/KaziJahidurRahaman/IndicesSgnificance/assets/109986838/06d6e3ce-0a45-4f53-a965-a5b8f1e10648)


## 4. Outputs
### 4.1 The class wise and overall accuracies for SVM, RF and ANN with 2 datasets

![image](https://github.com/KaziJahidurRahaman/IndicesSgnificance/assets/109986838/8e314669-dc1d-440e-9178-202d3ece6788)


### 4.2 Impact of indices on classwise and OA

![image](https://github.com/KaziJahidurRahaman/IndicesSgnificance/assets/109986838/d4bf5d78-0076-4d09-9749-f3d44f26341e)

### 4.3 Confusion Metrices of the algorithms with both datasets
![image](https://github.com/KaziJahidurRahaman/IndicesSgnificance/assets/109986838/bb23aba8-bf5f-427d-b96a-9c53a73334b7)
![image](https://github.com/KaziJahidurRahaman/IndicesSgnificance/assets/109986838/eebb2ae4-2f95-4976-a314-2fd092ae35fe)
![image](https://github.com/KaziJahidurRahaman/IndicesSgnificance/assets/109986838/6dd453e4-be1a-42f0-a5a2-93d23237854f)

### 4.4 Impact of the indices on time complexity of the models
#### 4.4.1 SVM's accuracy reduces with the indices, but computation time decreases significantly
![image](https://github.com/KaziJahidurRahaman/IndicesSgnificance/assets/109986838/765c3081-e7a3-41a7-b84b-96eebb77188d)

#### 4.4.2 RF and ANN gains accuracy when indices are added with data. But computation time increases
![image](https://github.com/KaziJahidurRahaman/IndicesSgnificance/assets/109986838/99f65308-af0b-438d-bc38-0b217faa8229)

#### 4.4.3 Learning Curves of ANN shows better ability to generalise when indices added
 
![image](https://github.com/KaziJahidurRahaman/IndicesSgnificance/assets/109986838/6094b551-d49c-4bae-9c24-fc89a05dad0a)

### 4.5 Proposed new approach performance and comaing with previous 2 best models shows better performance
![image](https://github.com/KaziJahidurRahaman/IndicesSgnificance/assets/109986838/b86e7505-be13-4e8c-ba35-4bc91d67573e)

![image](https://github.com/KaziJahidurRahaman/IndicesSgnificance/assets/109986838/317fceb8-ac61-42ec-955a-2b75ca542e61)

### 4.6 Classified LULC Maps
![image](https://github.com/KaziJahidurRahaman/IndicesSgnificance/assets/109986838/746fbe30-f5b7-4db9-9bae-618d6d09b3da)

![image](https://github.com/KaziJahidurRahaman/IndicesSgnificance/assets/109986838/3253bf66-b4ed-4dbf-9ad1-36721c8510b2)

![image](https://github.com/KaziJahidurRahaman/IndicesSgnificance/assets/109986838/e9280554-45dc-47c9-b48e-840a025b45aa)

![image](https://github.com/KaziJahidurRahaman/IndicesSgnificance/assets/109986838/a53581de-5ec3-4113-9587-7711a4b9375f)


## 5. Conclusion
<p>The study finds that, indices has diferring effects on various ML/DL algorithms, specially for DL algorithms, it improves the OA significantly. On the otherhand, it drops the accuracy of SVM algorithm, however, yet in this case, it significantly improves the computation complexity. As of the best algorithm to classiy the LULC is concerned, SVM with only the Band 1-12 is the opmtimal one. However, the newly proposed approach based best class wise models overtrumps the accuracy of SVM .</p>

##### [A detailed report of the task can be found in the report file. The classified outputs are availabale in the outputs folder].
