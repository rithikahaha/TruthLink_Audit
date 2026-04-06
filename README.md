# 🛡️ The Data Truth Audit: Finding the Lies in the Numbers

![Project Dashboard](dashboard.png)

### What is this project?
Imagine you are running a lemonade stand. At the end of the day, your notebook says you made ₹1,000. But when you count the cash in the box, you only have ₹800. 

**What happened?** Maybe you accidentally wrote down one sale twice. Maybe you forgot to count a refund. 

In the corporate world, this happens on a massive scale. This project is a **Truth Engine** I built to find those mistakes and show exactly how much they lie to a business.

### The Big Ouch Moments: What I found
I ran an audit on a dirty dataset and compared it to the actual truth. Here is how much the raw data lied to us:

**The Double Counting Trap**
The data said we made **20.7% more money** than we actually did. This happened because the system accidentally recorded some big sales twice. 

**The False Alarm Crisis**
The data said **33%** of customers were returning items. In reality, it was only **23%**. That is a **44.7% error.** A manager might fire a team over a 33% return rate, not realizing the data was just missing some Success checkmarks.

**The Price Blur**
A few massive, accidental price entries made the Average Sale look **11.7% higher** than it really was.

### How the Numbers were Calculated
To find these lies, I used a standard engineering formula to measure the **Distortion Gap** between the Raw Data and the verified Truth Data:

$$Distortion = \frac{Raw Value - Truth Value}{Truth Value} \times 100$$

**Example: Revenue Overstatement**
The raw system recorded ₹1,20,700 but the truth was ₹1,00,000. 
Calculation: ((1,20,700 - 1,00,000) / 1,00,000) * 100 = **+20.7%**

### How I Built It
I did not just find a random dataset. I **created** one so I could control the experiment:

1. **I Created the Truth:** I used Python to generate 1,000 perfect, clean sales records.
2. **I Broke the Data:** I intentionally added bugs—like duplicates and missing info—to simulate a messy real world system.
3. **I Fixed It:** I wrote code to find those bugs, clean them, and then calculated the gap between the lie and the truth.

### Tools I Used
* **Python:** The language I used to talk to the computer.
* **Pandas and NumPy:** My Data Calculators for handling big tables of numbers.
* **Seaborn:** The tool I used to draw the professional graphs in the dashboard.

### Why does this matter for a Data Analyst?
A great Data Analyst is a **detective**. This project proves that I have the detective skills to look at a report and ask: *Wait, is this number actually real, or is the data lying to us?*

### How to Run This Audit
1. **Clone this repository** to your local machine.
2. **Install dependencies:** `pip install pandas numpy matplotlib seaborn`
3. **Open the Notebook:** Open `TruthLink_Audit.ipynb` in VS Code or Jupyter.
4. **Run All Cells:** The audit will automatically generate the synthetic data and produce the Distortion Map.