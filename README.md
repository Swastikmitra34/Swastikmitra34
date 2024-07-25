## Hi there 👋


# Profile
# Swastik Mitra - Quantitative Analyst/Mathematician

Welcome to my GitHub profile! Here you'll find my projects and contributions related to quantitative analysis, artificial intelligence and actuarial science.

## Black-Scholes Equation

The Black-Scholes partial differential equation is:

$$
\frac{\partial V}{\partial t} + \frac{1}{2} \sigma^2 S^2 \frac{\partial^2 V}{\partial S^2} + r S \frac{\partial V}{\partial S} - r V = 0
$$
<div align="center">
  <img src="https://i.pinimg.com/originals/aa/e5/bc/aae5bc56711d59c0b490b07b3d386fa4.gif" alt="Animated Welcome" width="150">
</div>
And the solution for a European call option price \( C \) is given by:

$$
C(S, t) = S_0 \Phi(d_1) - K e^{-r(T-t)} \Phi(d_2)
$$

where

$$
d_1 = \frac{\ln\left(\frac{S_0}{K}\right) + \left(r + \frac{\sigma^2}{2}\right)(T-t)}{\sigma \sqrt{T-t}}
$$

and

$$
d_2 = d_1 - \sigma \sqrt{T-t}
$$


<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png" alt="JavaScript" height="50">
  <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" alt="Scikit-learn" height="50">
  <img src="https://upload.wikimedia.org/wikipedia/commons/0/0a/Python.svg" alt="Python" height="50">
  <img src="https://upload.wikimedia.org/wikipedia/commons/2/2d/Tensorflow_logo.svg" alt="TensorFlow" height="50">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRIfUYe1tSOIsRIhH6sLXqrqDoZHAKzzgE-lw&s" alt="Scikit-learn" height="50">
  <img src="https://upload.wikimedia.org/wikipedia/commons/1/1b/R_logo.svg" alt="R" height="50">
  <img src="https://upload.wikimedia.org/wikipedia/commons/1/18/C_Programming_Language.svg" alt="C" height="50">
  <img src="https://upload.wikimedia.org/wikipedia/commons/1/18/ISO_C%2B%2B_Logo.svg" alt="C++" height="50">
  <img src="https://user-images.githubusercontent.com/50221806/86498201-a8bd8680-bd39-11ea-9d08-66b610a8dc01.png" alt="numpy" height="50">
  <img src="https://geo-python-site.readthedocs.io/en/stable/_images/pandas_logo.png" alt="Pandas" height="50">
  <img src="https://studyopedia.com/wp-content/uploads/2023/07/scipy.png" alt="SciPy" height="50">
  <img src="https://upload.wikimedia.org/wikipedia/commons/8/84/Matplotlib_icon.svg" alt="Matplotlib" height="50">
  <img src="https://cdn.vectorstock.com/i/500p/96/95/cloud-iot-internet-of-things-icon-vector-22929695.jpg" alt="IoT" height="50">
  <img src="https://upload.wikimedia.org/wikipedia/commons/5/53/OpenCV_Logo_with_text.png" alt="OpenCV" height="50">
  <img src="https://seeklogo.com/images/J/jupyter-logo-A91705F539-seeklogo.com.png" alt="Jupyter" height="50">
  <img src="https://seeklogo.com/images/P/pytorch-logo-84F95D0AF5-seeklogo.com.png" alt="PyTorch" height="50">
  <img src="https://t3.ftcdn.net/jpg/04/36/20/28/360_F_436202824_9jWSKpjDrITJIVmkdBedp707rF5wLSjK.jpg" height="50">
  <img src="https://audioboom.com/i/35708601/600" height="50">
  <img src="https://upload.wikimedia.org/wikipedia/en/thumb/6/69/IIT_Madras_Logo.svg/800px-IIT_Madras_Logo.svg.png" height="50">
  
</p>

![Visitor Count](https://visitor-badge.laobi.icu/badge?page_id=Swastikmitra34.your-repo)

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Swastikmitra34&show_icons=true)

### [Financial Risk Model]

### [Financial Risk Model](https://github.com/Swastikmitra34/financial-risk-model)
A model to assess financial risk using Python.

```python

def create_life_table(age_data, mortality_rates):
    """
    Create a basic life table from age data and mortality rates.

    :param age_data: List of ages
    :param mortality_rates: List of mortality rates corresponding to each age
    :return: DataFrame containing the life table
    """
    # Create an empty DataFrame
    life_table = pd.DataFrame({'Age': age_data, 'Mortality Rate': mortality_rates})
    
    # Calculate qx (probability of death between age x and x+1)
    life_table['qx'] = life_table['Mortality Rate'].apply(lambda x: x / (1 + x))
    
    # Calculate lx (number of people alive at the beginning of each age x)
    life_table['lx'] = 100000  # Assuming an initial population of 100,000
    life_table['lx'] = life_table['lx'].shift(1) * (1 - life_table['qx'])
    life_table['lx'] = life_table['lx'].fillna(100000)
    
    # Calculate tx (total number of person-years lived from age x onward)
    life_table['tx'] = life_table['lx'].cumsum()
    
    # Calculate ex (life expectancy at age x)
    life_table['ex'] = life_table['tx'] / life_table['lx']
    
    return life_table

# Example data
ages = list(range(0, 101))  # Ages from 0 to 100
mortality_rates = [0.01] * 100 + [0.02]  # Example constant mortality rates

# Create life table
life_table_df = create_life_table(ages, mortality_rates)
print(life_table_df.head())
