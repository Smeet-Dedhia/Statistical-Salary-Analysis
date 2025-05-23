# 5. Predicting Academic Salaries: Can Data Science Forecast Your Paycheck?

Welcome to the final installment of our blog series on investigating faculty salary data at a US university. In this post, we would like to discuss about Predicting Academic Salaries using Machine Learning models and analyzing our findings.

---

Imagine you're a young assistant professor. You’ve spent years earning degrees, building expertise, and finally securing a faculty position. But one question lingers in your mind: How will your salary evolve over time? 

Will experience alone guarantee a bigger paycheck? Or do promotions, administrative roles, and even your field of study play a bigger role?  

To answer these questions, we built a **machine learning model** that predicts faculty salaries. What started as a curiosity-driven project soon turned into a deep dive into **career progression, academic hierarchies, and salary disparities**.  

Here’s what we discovered.  

## **The Data: More Than Just a Paycheck**  

Salary data isn’t just numbers—it’s a reflection of **career trajectories, institutional policies, and systemic patterns** in academia.  

For this project, we used historical faculty salary data, extracting key features that could influence earnings, including:  

**Field of Study** – Salaries vary significantly across disciplines.  
**Academic Rank** – Assistant, Associate, and Full Professors follow different salary paths.  
**Years in Rank** – Promotions often come with a **salary boost**, but how long does it take?  
**Administrative Roles** – Leadership positions tend to increase earnings.  
**Year of Degree & Start Year** – Seniority matters, but how much?  
**Highest Degree Earned** – Do some degrees command higher pay?  
**Year for Salary Prediction** – Users enter a future year to see how their salary might evolve.  

Armed with these features, we set out to build a model that could **forecast salaries and uncover hidden trends** in academic pay.  

---

## **Building the Prediction Model**  

To turn raw salary data into meaningful predictions, we chose **Lasso Regression**—a machine learning algorithm that **balances accuracy and interpretability**.  

### **Why Lasso Regression?**  
- **Feature Selection** – Lasso helps eliminate irrelevant variables, ensuring only the most important salary predictors remain.  
- **Efficiency** – It performs well even with **limited data** and avoids overfitting.  
- **Interpretability** – Unlike black-box models, Lasso allows us to **see which factors matter most** in salary prediction.  

The model was trained using historical salary records, **learning how faculty salaries change over time** based on career progression patterns.  

But what truly made this project exciting was not just forecasting paychecks—it was the **insights the model revealed**.  

---

## **What Drives Academic Salaries? Key Insights**  

### **Gender-Based Salary Comparison** 

Does gender affect academic salaries? The model predicts **separate salaries for male and female faculty members**, highlighting **potential pay disparities**.  

While factors like rank and experience still play a major role, **the results hint at systematic differences in pay** that merit further investigation.  

---

### **The Power of Promotions**  

How long does it take to move up the academic ladder?  

💡 According to the data, most **assistant professors are promoted after six years**—but salary growth isn’t always linear.  
💡 **Full professors** experience the largest salary jumps, reinforcing the importance of career advancement.  

This means **staying in the same rank for too long might hurt salary potential**, making promotions a crucial factor in long-term earnings.  

---

### **Administrative Roles: A Hidden Pay Boost?**

Professors who take on **administrative duties (e.g., department chairs)** tend to earn significantly more.  

Even if two faculty members have the **same years of experience**, one with an administrative role is likely to **have a higher salary trajectory**.  

So, if you’re an academic wondering whether to take on leadership responsibilities, this might be a **data-driven reason** to consider it!  

---

## **Beyond Predictions: Visualizing Salary Trends**  

One of the most valuable aspects of this project is not just the **predictions**, but the **insights the model reveals through data visualization**.  

**Feature Importance Visualization** – Inspired by SHAP, this chart shows **which variables influence salary the most**.  
**Career Progression Simulation** – Users can enter their **own academic qualifications** to see how their salary might evolve over time.  
**Model Performance Metrics** – The R² score provides a **clear measure of prediction accuracy**.  

These visualizations help transform raw numbers into a **story of career growth and salary potential**.  

---


[Here's the link to the prediction model](https://data557project-salarybias.streamlit.app/Model_Visualization)

---

## **Model Coeffecients**

![Coeffecient Barchart](/assets/blog4/coeffecients_chart.png)
![Coeffecient table](/assets/blog4/coeffecient_table.png)

Note: The coefficient for num_experience (15.1665) is not statistically significant at the 0.05 level, as its p-value is 0.1221, which is greater than 0.05. This suggests that num_experience does not have a significant impact on the dependent variable in this regression model.

---

## **Why This Matters**  

This project isn’t just about forecasting salaries—it’s about **empowering faculty members** to better understand their earning potential.  

**Aspiring professors** can use it to set salary expectations early in their careers.  
**Mid-career academics** can explore the impact of promotions and administrative roles.  
**Institutions** can use insights to **address salary disparities and improve policies**.  

At its core, **data science meets career strategy** in this project.  

---

## **What’s Next?**  

While the model provides valuable salary predictions, there’s always room for improvement.  

🔍 **Future Enhancements**:  
1. Expanding the dataset to include more institutions.  
2. Adding trend analysis across multiple years.  
3. Incorporating **inflation-adjusted salaries** for better accuracy.  
4. Exploring **AI-driven career recommendations** based on salary potential.  

For now, this project stands as a **practical, data-driven tool** for academics looking to navigate their career trajectories.  

## **Conclusion**  

As we wrap up this blog series, we hope you’ve gained valuable insights into the factors influencing academic salaries and how data science can be leveraged to predict and understand these trends. From exploring the nuances of career progression to uncovering potential disparities, our journey through faculty salary data has been both enlightening and thought-provoking. Thank you for joining us on this exploration, and we look forward to seeing how these insights might inspire positive changes in academia. Stay curious and keep questioning!