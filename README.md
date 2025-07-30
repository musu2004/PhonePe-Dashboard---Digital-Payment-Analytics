# 📱 **PhonePe Dashboard - Digital Payment Analytics**

## 📌 **Project Overview**
The **PhonePe Dashboard** provides comprehensive visualization of digital payment trends and transaction analytics across India. Built using **Power BI Desktop** and **MySQL**, this dashboard helps **fintech analysts, business strategists, and payment industry experts** understand transaction patterns, identify growth opportunities, and assess regional payment adoption. By leveraging this dashboard, organizations can make data-driven decisions to improve digital payment ecosystem and user engagement.

![PhonePe Dashboard](./screenshots/phonepe_dashboard.jpg)

---

## 📊 **Key Features**

### 1️⃣ **Total Transactions & Amount**
- **Objective**: Provide an overview of total transactions and transaction amounts across different time periods.
- **Output**: Metrics include **total transaction count**, **total transaction amount**, and **year-on-year growth trends**.

### 2️⃣ **Transaction Analysis by State**
- **Objective**: Analyze transaction patterns across different Indian states.
- **Output**: A **choropleth map** and **bar charts** showing transaction volumes and amounts by state.

### 3️⃣ **Payment Categories Breakdown**
- **Objective**: Understand transaction distribution across different payment categories.
- **Output**: **Pie charts** and **donut charts** breaking down transactions by categories like P2P, P2M, Recharge, etc.

### 4️⃣ **Top Districts Performance**
- **Objective**: Identify high-performing districts in terms of digital payment adoption.
- **Output**: **Ranked bar charts** showing top districts by transaction count and amount.

### 5️⃣ **Quarterly Trends Analysis**
- **Objective**: Track seasonal patterns and quarterly growth in digital payments.
- **Output**: **Line charts** and **area charts** showing quarterly transaction trends.

### 6️⃣ **User Demographics & Adoption**
- **Objective**: Analyze user registration and app opening trends.
- **Output**: **Heat maps** and **trend lines** showing user engagement patterns.

---

## 🛠️ **Technology Stack**

### **Data Storage & Management**
- **MySQL 8.0** - Primary database for storing transaction data
- **MySQL Connector/ODBC** - Database connectivity
- **Python 3.8+** - Data processing and ETL operations

### **Visualization & Analytics**
- **Microsoft Power BI Desktop** - Primary dashboard creation tool
- **Power Query** - Data transformation and cleaning
- **DAX (Data Analysis Expressions)** - Custom calculations and measures

### **Data Processing**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **SQLAlchemy** - Database ORM and connection management
- **Matplotlib/Seaborn** - Additional data visualization support

---

## ⚙️ **Setup Instructions**

### 🔹 **Step 1: Clone the Repository**
```bash
git clone https://github.com/yourusername/PhonePe-Dashboard.git
cd PhonePe-Dashboard
```

### 🔹 **Step 2: Install Python Dependencies**
```bash
pip install -r requirements.txt
```

### 🔹 **Step 3: Setup MySQL Database**
```bash
# Install MySQL (if not already installed)
brew install mysql  # For macOS
# Start MySQL service
brew services start mysql

# Create database and import schema
mysql -u root -p < database/schema/phonepe_schema.sql
```

### 🔹 **Step 4: Configure Database Connection**
```bash
# Copy and edit configuration file
cp python/config/config.template.py python/config/config.py
# Edit config.py with your MySQL credentials
```

### 🔹 **Step 5: Load Sample Data**
```bash
python python/data_processing/load_phonepe_data.py
```

### 🔹 **Step 6: Open Power BI Dashboard**
1. Install **Microsoft Power BI Desktop**
2. Open `powerbi/PhonePe_Dashboard.pbix`
3. Update data source connections to point to your MySQL database
4. Refresh data and explore the dashboard

---

## 📈 **Dashboard Features Detailed**

### **Transaction Analytics**
- Real-time transaction monitoring
- State-wise transaction heatmaps
- Category-wise transaction breakdown
- Trend analysis with forecasting

### **Geographic Insights**
- Interactive maps showing transaction density
- State and district-level performance metrics
- Regional growth patterns and comparisons

### **User Engagement Metrics**
- App downloads and user registrations
- Active user trends and retention analysis
- Demographic breakdowns and user behavior

### **Financial Metrics**
- Transaction volume and value trends
- Average transaction amounts
- Peak transaction periods and patterns

---

## 🔄 **Data Sources**

### **PhonePe Pulse Data**
- Transaction data by state and district
- User registration and app opening data
- Payment category breakdowns
- Quarterly and yearly aggregations

### **External Data Sources**
- Indian state and district geographic data
- Population and demographic information
- Economic indicators for correlation analysis

---

## 🚀 **Future Enhancements**

### 🔹 **Real-Time Data Integration**
- **Objective**: Implement real-time transaction monitoring
- **Method**: Integrate with PhonePe APIs for live data feeds

### 🔹 **Machine Learning Predictions**
- **Objective**: Predict transaction trends and user behavior
- **Method**: Implement ML models for forecasting and anomaly detection

### 🔹 **Advanced Analytics**
- **Objective**: Deep-dive analysis with advanced statistical methods
- **Method**: Implement cohort analysis, customer segmentation, and churn prediction

### 🔹 **Mobile Dashboard**
- **Objective**: Create mobile-responsive dashboard version
- **Method**: Develop Power BI mobile app integration and responsive design

---

## 📊 **Key Performance Indicators (KPIs)**

### **Transaction Metrics**
- Total Transaction Count
- Total Transaction Amount (₹)
- Average Transaction Value
- Transaction Success Rate

### **Growth Metrics**
- Month-over-Month Growth
- Year-over-Year Growth
- Quarter-over-Quarter Growth
- Compound Annual Growth Rate (CAGR)

### **User Metrics**
- Total Registered Users
- Active Monthly Users
- User Retention Rate
- App Download Trends

### **Geographic Metrics**
- State-wise Market Share
- District Penetration Rate
- Urban vs Rural Adoption
- Regional Growth Patterns

---

## 🔧 **Troubleshooting**

### **Common Issues**
1. **Database Connection Error**: Check MySQL service and credentials
2. **Power BI Data Refresh Error**: Verify ODBC driver installation
3. **Python Package Issues**: Update pip and reinstall requirements
4. **Large Dataset Loading**: Consider data sampling for testing

### **Performance Optimization**
- Use indexed columns for faster queries
- Implement data partitioning for large datasets
- Cache frequently accessed data
- Optimize Power BI relationships and calculations

---

## 🤝 **Contributing**

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 **Author**

**Your Name**
- GitHub: [musu2004](https://github.com/musu2004)
- LinkedIn: [muskanshaw20](https://linkedin.com/in/muskanshaw20)
- Email: muskaanshaw2010@gmail.com

---

## 🙏 **Acknowledgments**

- **PhonePe** for providing open data through PhonePe Pulse
- **Microsoft** for Power BI Desktop
- **MySQL** community for database support
- **Python** community for amazing libraries and tools
