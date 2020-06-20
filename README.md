# Medium-Writing_earning-analysis
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/satan87/Medium-Writing_earning-analysis/master)

Jupyter Notebook to analize Medium earning.


You need to update your data
#### TAX RATE


```python
Tax = 0.7
```

#### YOUR STORIES


```python
class Stories(Enum):
    STORY_1_TITLE = Story("My First Story", 500, 3)
    STORY_2_TITLE = Story("My Second Story", 1000, 5)
```

#### YOUR GAINS


```python
gains = [
    Gain(Stories.STORY_1_TITLE, Platform.Medium, Month.January, 2020, 8.00),
    Gain(Stories.STORY_1_TITLE, Platform.Medium, Month.February, 2020, 9.00),
    Gain(Stories.STORY_1_TITLE, Platform.Medium, Month.March, 2020, 7.00),
    Gain(Stories.STORY_2_TITLE, Platform.Medium, Month.March, 2020, 3.00),
    Gain(Stories.STORY_1_TITLE, Platform.Medium, Month.May, 2020, 9.00),
    Gain(Stories.STORY_2_TITLE, Platform.Medium, Month.May, 2020, 10.00),
    Gain(Stories.STORY_1_TITLE, Platform.Medium, Month.June, 2020, 11.00),
    Gain(Stories.STORY_2_TITLE, Platform.Medium, Month.June, 2020, 7.00)
]
```

It will display for you 3 metrics:
#### -- TOTAL GAIN PER YEAR --
#### -- TOTAL GAIN PER YEAR / PER MONTH --
#### -- TOTAL GAIN PER STORY --
