Project Overview: Business Lead Generation for a Marketing Agency

Our project embarked on a journey to gather business leads for a marketing agency renowned for its team of copywriters and content writers with over 15 years of experience. This team's expertise lies in amplifying social media engagement and driving the sales of products and services. Here’s the story of how we did it.

---

In the bustling world of social media and online marketing, our agency recognized a golden opportunity. We knew that small to medium-sized businesses often struggle to make their mark in the digital space, despite their best efforts. With this in mind, we set out to identify and assist these hidden gems, bringing our seasoned marketing magic to their doorsteps.

Phase 1: Setting the Stage

We began by zeroing in on companies within specific industries: marketing tech, fitness tech, solar energy, roofing, home remodeling, and general contracting. These sectors were chosen not only for their growth potential but also for the unique marketing challenges they face. Our geographical focus was on vibrant business hubs across the USA, such as Denver, Colorado; San Jose; Austin, Texas; Dallas, Texas; and Phoenix. These regions, teeming with entrepreneurial spirit, offered a fertile ground for our endeavors. Additionally, we targeted businesses with no more than 200 employees, aiming to support startups and small to medium-sized enterprises.

Phase 2: Gathering Intelligence

With our targets defined, we deployed a Python script to scour LinkedIn for relevant data. We meticulously gathered information on company names, websites, founding years, company sizes, and headquarters locations. Our digital net captured around 1,000 companies, each a potential beneficiary of our expertise.

Phase 3: The Instagram Quest

Next, we turned our attention to Instagram, the social media powerhouse. From company websites, we verified whether they had Instagram accounts. For those that did, we scraped valuable data: follower counts, last post dates, likes, and comments. This step was crucial in understanding their current social media engagement.

Phase 4: Sifting for Gems

Armed with Instagram data, we focused on companies that were actively posting but struggling to gain traction. These businesses, we knew, were keen on boosting their social media presence but needed the right push. We further validated their potential by checking Google reviews, ensuring they had quality products and services, yet faced challenges in reaching a broader audience.

Phase 5: Connecting the Dots

From this refined list, we turned to Apollo to gather detailed contact information. Emails, phone numbers, names, and roles within these companies were carefully compiled. By the end, we had identified 22 prime leads: 11 in solar energy, 2 in fitness tech, 3 in roofing, 4 in general contracting, 1 in marketing tech, and 1 in home remodeling.

Phase 6: The Power of Prediction

As a final touch, we harnessed the power of machine learning. Our beta model analyzed Instagram metrics—followers, likes, comments, and posting activity—alongside business model data. The model flagged companies that, despite recent activity, had low engagement, highlighting them as ideal candidates for our services.

---

Through this structured yet dynamic approach, we not only identified businesses in need but also demonstrated our agency’s capability to turn social media struggles into success stories. This project underscored our commitment to helping small and medium-sized enterprises thrive in the digital age, leveraging our unparalleled expertise to drive engagement and sales.

---

Technical Overview: Machine Learning Model Development

After filtering our data, we moved to the preprocessing phase and began manually verifying and labeling companies according to their business models. However, we quickly encountered a challenge: there was insufficient data on companies with good social media engagement. To address this, we took several technical steps:

Data Augmentation:

1. Synthetic Data Generation:
   - Followers: Generated random follower counts between 3,000 and 25,000.
   - Last Post Interactions: Set interactions (likes) to range between 5% and 18% of the follower count.
   - Comments: Assigned comments to range between 5% and 10% of the follower count.

2. Addressing Data Imbalance:
   - Despite generating synthetic data, our dataset remained small.
   - Applied Synthetic Minority Over-sampling Technique (SMOTE) to oversample the minority class, ensuring a more balanced dataset.

Model Development:

3. Model Selection:
   - Chose AdaBoosting with a Decision Tree estimator due to its robustness and ability to handle our varied data.

4. Hyperparameter Tuning:
   - Utilized GridSearchCV to fine-tune the model’s parameters, optimizing its performance.

Model Evaluation:

5. Performance Metrics:
   - Achieved 100% accuracy, precision, and recall on both training and test datasets.
   - Although these results suggest overfitting, the model performed as expected given the small dataset size.

By generating synthetic data and using advanced techniques like SMOTE and GridSearchCV, we built a model capable of identifying companies with low engagement but recent activity. This model is a critical tool in pinpointing businesses that could benefit from our marketing agency's expertise.

