# Data
-   **Hot Ones Episodes Dataset**: 
Hot Ones is an American YouTube talk show, created by Chris Schonberger, hosted by Sean Evans and produced by First We Feast and Complex Media. Its basic premise involves celebrities being interviewed by Evans over a platter of increasingly spicy chicken wings.

# Codebook for Hot Ones Dataset

## Variable Names and Descriptions:

### `episodes.csv`
|Variable Name           |Description             |
|:-----------------------|:-----------------------|
|season                  |The season number.      |
|episode_overall         |The overall count of this episode, from 1-300.|
|episode_season          |The count of this episode within this season.|
|title                   |The title of the episode.|
|original_release        |The date on which the episode was originally available on YouTube.|
|guest                   |The name of the guest. |
|guest_appearance_number |The number of appearances by this guest so far as of this date. |
|finished                |Whether the guest finished trying all of the sauces. |

### `sauces.csv`

|Variable Name|Description  |
|:------------|:------------|
|season       |The season number. |
|sauce_number |The number of this sauce, from 1 (least hot) to 10 (hottest). |
|sauce_name   |The name of the sauce. |
|scoville     |The rating of the sauce in [Scoville heat units](https://en.wikipedia.org/wiki/Scoville_scale). |

### `seasons.csv`

|Variable Name    |Description      |
|:----------------|:----------------|
|season           |The season number. |
|episodes         |The count of episodes in this season. |
|note             |Notes about this season. |
|original_release |The date of the first episode in this season. |
|last_release     |The date of the last episode of this season (if that episode has aired at the time of scraping). |

## Data Types:

### `episodes.csv`

|Column                  |Datatype  |
|:-----------------------|:---------|
|season                  |integer   |
|episode_overall         |integer   |
|episode_season          |integer   |
|title                   |character |
|original_release        |date      |
|guest                   |character |
|guest_appearance_number |integer   |
|finished                |logical   |

### `sauces.csv`

|Column       |Datatype  |
|:------------|:---------|
|season       |integer   |
|sauce_number |integer   |
|sauce_name   |character |
|scoville     |integer   |

### `seasons.csv`

|Column           |Datatype  |
|:----------------|:---------|
|season           |integer   |
|episodes         |integer   |
|note             |character |
|original_release |date      |
|last_release     |date      |