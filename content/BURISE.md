+++
title = 'BU RISE'
description = "Here is my project for the BU RISE 2024 summer program, which culminated in an abstract and a poster."
draft = false
+++
Research project for the BU RISE 2024 summer program, culminated in an abstract and a poster. 

### **<p style="text-align: center;">Temperature Prediction in Monolithic 3D Using Machine Learning Based Models</p>**

<p style="text-align: center;">Alan Zhou<sup>1,2</sup>; Amin Khodaverdian<sup>2</sup>; Ayse K. Coskun<sup>2</sup> </p>

<p style="text-align: center;"><sup>1</sup>Episcopal Academy, 1785 Bishop White Drive, Newtown Square, PA 19073; <sup>2</sup>Department of Electrical & Computer Engineering, Boston University, 8 St. Mary’s Street, Boston, MA 02215</p>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;High chip temperatures have been a key issue for decades. In conventional chip designs, high temperatures negatively impact performance and can degrade the lifetime of processors [1]. Monolithic 3D(M3D) integration is an emerging technology enabling the stacking of multiple transistor, or active, layers(we also refer to these layers as tiers) within one Integrated Circuit(IC). M3D serves as an alternative to traditional transistor scaling by providing vertical interconnects between transistor layers, allowing for dense ICs and high bandwidth communication between layers [2]. As a result of various factors, M3D systems face additional thermal issues compared to traditional designs, making thermal management a critical issue [3]. Runtime thermal management policies provide one way to alleviate thermal issues. However, current policies rely on temperature readings from on-chip thermal sensors, which may not provide accurate measurements for maximum temperatures on the chip, a consequence of several limitations of these sensors [1]. We expanded upon previous work [1] to develop a nonlinear regression model, trained and evaluated on data generated from simulations, to predict the on-chip temperatures for active layers in a two-tiered M3D processor, The goal is to predict an output from PACT, a compact thermal simulator, which is a full temperature node grid for each active layer, in our case a 100x100 sized node grid. Our proposed model is a Decision Tree Multi Regression model from the Scikit Learn python library with default hyperparameters. As input, the proposed model takes in on-chip temperature sensor readings; the location of the sensor inputs; and the total power usage of the layer divided by the size of the temperature grid. The proposed model outputs an array of temperature values which correspond onto a 100x100 temperature grid. Giving the model 20 temperature readings, we achieved a maximum R^2 score of approximately 0.871.   

**References:**

[1] Knox, C, Yuan, Z, & Coskun, AK. "Machine Learning and Simulation Based Temperature Prediction on High-Performance Processors." Proceedings of the ASME 2022 International Technical Conference and Exhibition on Packaging and Integration of Electronic and Photonic Microsystems. ASME 2022 International Technical Conference and Exhibition on Packaging and Integration of Electronic and Photonic Microsystems. Garden Grove, California, USA. October 25–27, 2022. V001T05A001. pp 1.   
[2] K. Dhananjay, P. Shukla, V. F. Pavlidis, A. Coskun and E. Salman, "Monolithic 3D Integrated Circuits: Recent Trends and Future Prospects," in IEEE Transactions on Circuits and Systems II: Express Briefs, vol. 68, no. 3, pp. 837-843, March 2021, doi: 10.1109/TCSII.2021.3051250. pp 1   
[3]. P. Shukla, A. K. Coskun, V. F. Pavlidis, and E. Salman, “An overview of thermal challenges and opportunities for monolithic 3D ICs,” in Proceedings of the 2019 on Great Lakes Symposium on VLSI, 2019, pp. 439–444. pp 2.


![poster](/images/Zhou,Alan.Poster.png "100%")


