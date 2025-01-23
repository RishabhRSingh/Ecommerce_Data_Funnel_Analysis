# **Conversion Analysis and Funnel Optimization**

## **Project Overview**
This project analyzes user behavior across a website’s conversion funnel using data from multiple stages. By leveraging Python and Jupyter Notebook, we calculate conversion rates, identify bottlenecks, and provide actionable insights to improve the user journey.

---

## **Data Files**
The analysis is based on the following CSV datasets:

1. **`user_table.csv`**  
   - Contains user details:  
     - `date`: Date of activity.  
     - `user-id`: Unique identifier for users.  
     - `sex`: User's gender.  
     - `device-used`: Device used to access the website (mobile, desktop, etc.).

2. **`home_page_table.csv`**  
   - User-IDs of users who visited the home page.

3. **`search_page_table.csv`**  
   - User-IDs of users who visited the search page.

4. **`payment_page_table.csv`**  
   - User-IDs of users who visited the payment page.

5. **`payment_confirmation_table.csv`**  
   - User-IDs of users who successfully completed payment and received confirmation.

---

## **Analysis Steps**
The project is structured in a Jupyter Notebook for seamless analysis, combining data manipulation, visualization, and insights generation.

### **1. Funnel Visualization**  
Using **Plotly**, we create a funnel chart to track user drop-offs at each stage:  
- **Home Page → Search Page → Payment Page → Payment Confirmation Page**  

#### **Key Conversion Rates**:
1. **Search → Payment Page**: Only **7%** conversion rate.  
2. **Payment → Confirmation Page**: Only **1%** conversion rate.

---

### **2. Identified Issues**
#### Between **Search Page** and **Payment Page**:  
- Unclear product details or high pricing may discourage users.  
- Payment options or interface friction might contribute to drop-offs.

#### Between **Payment Page** and **Confirmation Page**:  
- Payment errors or trust issues could be causing the significant drop-offs.  

---

### **3. Recommendations**
#### **Improve Search Experience**:
- Optimize filters and suggestions.  
- Highlight promotions or discounts to engage users.

#### **Enhance Payment Process**:
- Simplify payment flows and offer diverse, secure payment methods.  

#### **Follow-Up on Abandoned Payments**:
- Use reminders and incentives to re-engage users who abandon payments.  

#### **Analyze User Feedback**:
- Regularly gather and address feedback to resolve pain points.  

---

### **4. Segmentation Insights**
Data was merged and segmented, with results visualized using **funnel and pie charts**.

#### **Key Insights**:
1. **Mobile Dominance**:  
   - Mobile users account for **66.8%** of conversions.    

2. **Desktop Lagging**:  
   - Desktop users contribute only **33.2%**, signaling optimization opportunities.  

3. **Female Preference**:  
   - Female users (53.3%) slightly outperform male users (46.7%) in conversions.  

#### **Recommendations**:
1. **Focus on Mobile**:  
   - Enhance mobile user experience.  

2. **Boost Desktop Performance**:  
   - Address desktop-specific challenges and retarget users with incentives.  

3. **Targeted Campaigns**:  
   - Create strategies based on the female audience preference while attracting male users.  

---

### **5. Time Series Analysis**
Using **Plotly line graphs**, we analyzed daily conversion rates and identified:  
- A **major drop** in conversion rates from the **home page to search page** on **mobile devices**, decreasing from **0.8** to **0.2** on 1st March in the data.  

#### **Recommendations**:
- Investigate causes for mobile-specific drop-offs.  
- Improve mobile product discoverability, page load speeds, and user experience.

---

## **Technical Stack**
- **Environment**: Jupyter Notebook  
- **Languages**: Python  
- **Libraries**: Pandas, Plotly, Matplotlib  
- **Visualizations**: Funnel Charts, Pie Charts, Line Graphs  
- **Analysis**: Conversion Metrics, Time Series Analysis  

---

## **How to Run the Notebook**
1. Clone the project repository.  
2. Install the required Python libraries using the following command:  
   ```bash
   pip install pandas plotly matplotlib
   ```
3. Place the CSV files in the project directory.  
4. Open the Jupyter Notebook and execute the cells sequentially to preprocess data, visualize the funnel, and extract insights.

---

## **Future Scope**
- Add A/B testing results to evaluate UX changes.  
- Cluster users to create more personalized marketing strategies.  
- Include geographic and demographic data for deeper segmentation.  

