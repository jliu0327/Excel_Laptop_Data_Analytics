# Excel Laptop Data Analytics

https://github.com/user-attachments/assets/b35ed6f8-423f-4c0f-8db7-b54384be1c0e

## Introduction
This laptop pricing dashboard was created to aid consumers in deciding the type of laptop they want to purchase, based on multiple factors and average pricing of the laptops.

The data came from the kaggle dataset: [Laptop Pricing Dataset](https://www.kaggle.com/datasets/asinow/laptop-price-dataset), and provides detailed information that are important when deciding on a new laptop.

### Dashboard File

My final dashboard is in [Excel_Laptop_Data_Analytics](Excel_Laptop_Data_Analytics)  

### Excel Skills Used

The following Excel skills were utilized for analysis:

- **Charts**
- **Formulas and Functions**
- **Data Validation**

### Laptop Dataset

As mentioned, the dataset used for this project came from kaggle, and includes detailed information on:

- **Brands**
- **CPU Processor**
- **GPU**
- **Price**

## Dashboard Build

### Charts  

**Laptop Brand Prices - Bar Chart**  
<img width="487" alt="Laptop_Brand_Prices _Bar_Chart" src="https://github.com/user-attachments/assets/7cde4c21-c31b-45f2-b1b7-075535dd47cd" />

- **Excel Features:** Utilized bar chart feature and optimzed layout for clarity
- **Design Choice:** Horizontal bar chart for visual comparison of average prices
- **Data Organization:** Sorted laptop brands by descending salary for improved readability
- **Insights Gained:** This enables quick identification of pricing trends, indicating that MSI and Apple cost the most compared to other laptop brands

### Formulas and Functions

**Average Prices by GPU**
```excel
=AVERAGE(
      IF(
         (laptops[Brand]=brand_name)*
         (laptops[Price ($)]<>0)*
         (laptops[Processor]=processor_name)*
         (laptops[GPU]=A2),
          laptops[Price ($)]
      )
)
```
- **Multi-Criteria Filtering:** Checks laptop brand, cpu, gpu, and excludes prices that are blank
- **Array Formula:** Utilizes ```AVERAGE()``` function with nested ```IF``` statement
- **Insights Gained:** Provides specific pricing information, depending on brand, cpu, and gpu 



## Laptop Price Analysis

With the current economy, there is no secret that prices are surging higher than ever. As a consumer and enthusiast of technology, such as laptops, I was fascinated to look into the priciing of different laptops, based on the different specs that came with it, and to compare it with other brands to see whiich laptops are worth more than others. 





