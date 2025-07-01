<h2>📈 Business Lead Generation for a Marketing Agency</h2>
Overview
This project was designed to generate high-quality business leads for a marketing agency with over 15 years of experience in copywriting and content marketing. The agency specializes in increasing social media engagement and driving sales for products and services. Our mission: identify businesses with strong offerings but weak digital presence—and connect them with the right help.

<h3>🚀 Project Goals</h3>
Identify small to medium-sized businesses (SMBs) with underperforming social media.

Focus on companies likely to benefit from expert marketing services.

Build a data-driven lead generation pipeline using Python, web scraping, and machine learning.

<h3>🧭 Target Criteria</h3>
Industries: Marketing Tech, Fitness Tech, Solar Energy, Roofing, Home Remodeling, General Contracting

Location: USA-based businesses, especially in:

Denver, CO

San Jose, CA

Austin & Dallas, TX

Phoenix, AZ

Size: Fewer than 200 employees

---

<h2>📊 Project Workflow</h2>

<h3>🔹 Phase 1: Industry & Region Targeting</h3>
Defined industries and U.S. business hubs most likely to need marketing help. Focused on regions rich in entrepreneurship.

<h3>🔹 Phase 2: LinkedIn Scraping</h3>
Used Python scripts to gather:

Company names

Websites

Founding years

Team sizes

Headquarters locations
📦 Result: ~1,000 potential business leads collected

<h3>🔹 Phase 3: Instagram Analysis</h3>
Extracted Instagram engagement metrics for each company:

Follower count

Last post date

Likes and comments

<h3>🔹 Phase 4: Lead Qualification</h3>
Selected companies that:

Were actively posting

Had low engagement

Had strong Google reviews (indicating good service/product)

<h3>🔹 Phase 5: Contact Info Enrichment</h3>
Used Apollo.io to enrich leads with:

Emails

Phone numbers

Key team members (names, roles)

<h3>📌 Final Output: 22 qualified leads</h3>

Solar Energy: 11

Fitness Tech: 2

Roofing: 3

General Contracting: 4

Marketing Tech: 1

Home Remodeling: 1

---
<h2>🤖 Machine Learning Component</h2>
To scale and refine lead selection, we built a classification model that predicts which companies are strong candidates for social media help.

<h3>📁 Data Preprocessing</h3>
Manually labeled companies based on engagement and business models

Noted lack of high-engagement data

<h3>🧪 Data Augmentation</h3>
Synthetic Data Generation

Followers: Randomly generated [3,000–25,000]

Likes: 5–18% of follower count

Comments: 5–10% of follower count

Imbalanced Data Handling

Applied SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset

<h3>🛠 Model Development</h3>
Model Chosen: AdaBoostClassifier with DecisionTree base estimator
(Chosen for its performance on small, noisy datasets)

Hyperparameter Tuning:
Used GridSearchCV for optimal settings

<h3>📈 Model Evaluation</h3>
Achieved 100% accuracy, precision, and recall on both training and test sets
⚠️ Note: High performance due to small dataset; potential overfitting acknowledged
