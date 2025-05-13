# csc412-project--data-cleaning-solved
**TO GET THIS SOLUTION VISIT:** [CSC412 Project- Data Cleaning Solved](https://www.ankitcodinghub.com/product/csc412-project-data-cleaning-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;94044&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSC412 Project- Data Cleaning Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
In Bb you will find a dataset from the UCI Machine Learning Repository on whether a patient has heart disease. You will clean the data and then apply a decision tree to the data.

<ol>
<li>As we did with the credit card data, load the data using pandas and import all modules that you may need.</li>
<li>Print the first 5 rows of the dataset.</li>
<li>You should see that column names, we just have column numbers. Since column names
would make it easier to know how to format the data, let’s replace the column numbers with column names:

df.columns = [‘age’, ‘sex’,

‘cp’, ‘restbp’, ‘chol’, ‘fbs’, ‘restecg’, ‘thalach’, ‘exang’, ‘oldpeak’, ‘slope’, ‘ca’, ‘thal’, ‘hd’]
</li>
<li>Determine the datatype of each column</li>
<li>We see that that they are almost all `float64`, however, two columns, “ca” and “thal”,
have the `object` type and one column, “hd” has `int64`.
</li>
</ol>
The fact that the **ca** and **thal** columns have `object` data types suggests there is something funny going on in them. `object` datatypes are used when there are mixtures of things, like a mixture of numbers and letters. In theory, both **ca** and **thal** should just have a few values representing different categories.

Print out the unique values for these columns.

<ol start="6">
<li>Column **ca** contains numbers (0.0, 3.0, 2.0 and 1.0) and questions marks (?). The numbers represent the number of blood vessels that were lit up by fluoroscopy and the question marks represent missing data.</li>
<li>Column “thal” also contains a mixture of numbers, representing the different diagnoses from the thalium heart scan, and question marks, which represent missing values.</li>
<li>Determine how many rows contain missing values. The python code is below. len(df.loc[(df[‘ca’] == ‘?’) | (df[‘thal’] == ‘?’)])</li>
<li>Since only 6 rows have missing values, let’s look at them.</li>
</ol>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
df.loc[(df[‘ca’] == ‘?’) | (df[‘thal’] == ‘?’)]

<ol start="10">
<li>Count the number of rows in the full dataset.</li>
<li>Remove the rows with missing values</li>
<li>Verify that you removed the rows by printing the size of the dataset.</li>
<li>Verify using the unique function that “ca” and “thal” do not have missing values.</li>
<li>Split the Data into Dependent and Independent Variables
<ol>
<li>The columns of data that we will use to make classifications</li>
<li>The column of data that we want to predict.</li>
</ol>
Use `copy()` to copy the data *by value* as we did with the credit card data.
</li>
<li>Print the head of both the X and y dataframes so that you can verify this worked correctly</li>
</ol>
# # Format the Data Part 2: One-Hot Encoding

#

# Now that we have split the data frame into two pieces, `X`, which contains the data we will use to make, or predict, classifications, and `y`, which contains the known classifications in our training dataset, we need to take a closer look at the variables in `X`. The list bellow tells us what each variable represents and the type of data (**float** or **categorical**) it should contain:

#

<ul>
<li># &nbsp;– **age**, **Float**</li>
<li># &nbsp;– **sex** – **Category**</li>
<li># &nbsp;– 0 = female</li>
<li># &nbsp;– 1 = male</li>
<li># &nbsp;– **cp**, chest pain, **Category**</li>
<li># &nbsp;– 1 = typical angina</li>
<li># &nbsp;– 2 = atypical angina</li>
<li># &nbsp;– 3 = non-anginal pain</li>
<li># &nbsp;– 4 = asymptomatic</li>
<li># &nbsp;– **restbp**, resting blood pressure (in mm Hg), **Float**</li>
<li># &nbsp;– **chol**, serum cholesterol in mg/dl, **Float**</li>
<li># &nbsp;– **fbs**, fasting blood sugar, **Category**</li>
<li># &nbsp;– 0 = &gt;=120 mg/dl</li>
<li># &nbsp;– 1 = &lt;120 mg/dl</li>
<li># &nbsp;– **restecg**, resting electrocardiographic results, **Category**</li>
<li># &nbsp;– 1 = normal</li>
<li># &nbsp;– 2 = having ST-T wave abnormality</li>
<li># &nbsp;– 3 = showing probable or definite left ventricular hypertrophy</li>
<li># &nbsp;– **thalach**, maximum heart rate achieved, **Float**</li>
<li># &nbsp;– **exang**, exercise induced angina, **Category**</li>
<li># &nbsp;– 0 = no</li>
<li># &nbsp;– 1 = yes</li>
<li># &nbsp;– **oldpeak**, ST depression induced by exercise relative to rest. **Float**</li>
<li># &nbsp;– **slope**, the slope of the peak exercise ST segment, **Category**</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
<ul>
<li># &nbsp;– 1 = upsloping</li>
<li># &nbsp;– 2 = flat</li>
<li># &nbsp;– 3 = downsloping</li>
<li># &nbsp;– **ca**, number of major vessels (0-3) colored by fluoroscopy, **Float**</li>
<li># &nbsp;– **thal**, thalium heart scan, **Category**</li>
<li># &nbsp;– 3 = normal (no cold spots)</li>
<li># &nbsp;– 6 = fixed defect (cold spots during rest and exercise)</li>
<li># &nbsp;– 7 = reversible defect (when cold spots only appear during exercise) #
16. Verify that the columns that are categorical contains the correct data values. Then use one hot encoding to separate the columns “cp”, “restecg”, “slope”. and “thal” so that each resulting column only contains “0s” and “1s”.

Use the same method we used in the credit card data.

X_encoded = pd.get_dummies(X, columns=[‘cp’, ‘restecg’,

‘slope’, ‘thal’])

X_encoded.head()

The 3 categorical columns that only contain 0’s and 1’s: sex, fbs (fasting blood sugar), and exang (exercise induced angina) don’t need any special treatment. As we can see, “”One-Hot Encoding”” converts a column with more than two categories, like “cp” (chest pain) into multiple columns of “0”s and “1”s. Since “sex”, “fbs”, and “exang” only have “2” categories and only contain “0”s and “1”s to begin with, we do not have to do anything special to them, so we’re done formatting the data.

<ol start="17">
<li>Now, one last thing before we run the data in a classification model, `y` doesn’t just contain “0”s and “1”s. Instead, it has “5” different levels of heart disease. “0 =“ no heart disease and “1-4” are various degrees of heart disease. We can see this with `unique()`:
y.unique()

Since we’re only doing a binary classification, and only care if someone has heart disease or not, we need to convert all numbers “&gt; 0” to “1”.

y_not_zero_idx = y &gt; 0 y[y_not_zero_idx] = 1 y.unique()
</li>
<li>Use this data to run a decision tree on the data. Determine how many levels the tree needs in order to accurately predict on “new” data.</li>
</ol>
</li>
</ul>
</div>
</div>
</div>
