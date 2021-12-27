# 🐕 I love dogs 🐶  

Data in this repository comes from the [American Kennel Club](https://www.akc.org/).

<img src="https://media-cldnry.s-nbcnews.com/image/upload/newscms/2020_28/1587661/dogs-age-years-kb-inline-200707.jpg" alt="image of five puppies sitting and looking at camera with a white background" width="300" >

## The Datasets

- `breed_traits_long` - trait information on each dog breed and scores for each trait (long format)
- `breed_traits` - trait information on each dog breed and scores for each trait (wide format)
- `trait_description` - long descriptions of each trait and values corresponding to `Trait_Score`
- `breed_rank_all` - popularity of dog breeds by AKC registration statistics from 2013-2020


## Data Dictionary

### `breed_traits_long.csv`

|variable        |class     |description |
|:---------------|:---------|:-----------|
|Breed    |character | Dog Breed |
|Trait            |character | Name of trait/characteristic |
|Trait_Score            |character    | Placement on scale of 1-5 for the trait, with the exception of a description for coat type and length

### `breed_traits.csv`

|variable        |class     |description |
|:---------------|:---------|:-----------|
|Breed    |character | Dog Breed |
|Affectionate With Family            |character | Placement on scale of 1-5 for the breed's tendancy to be "Affectionate With Family" (Trait_Score) |
|Good With Young Children            |character | Placement on scale of 1-5 for the breed's tendancy to be "Good With Young Children" (Trait_Score) |
|Good With Other Dogs          |character | Placement on scale of 1-5 for the breed's tendancy to be "Good With Other Dogs" (Trait_Score) |
|Shedding Level          |character | Placement on scale of 1-5 for the breed's "Shedding Level" (Trait_Score) |
|Coat Grooming Frequency         |character | Placement on scale of 1-5 for the breed's "Coat Grooming Frequency" (Trait_Score) |
|Drooling Level         |character | Placement on scale of 1-5 for the breed's "Drooling Level" (Trait_Score) |
|Coat Type         |character | Description of the breed's coat type (Trait_Score) |
|Coat Length         |character | Description of the breed's coat length (Trait_Score) |
|Openness To Strangers            |character | Placement on scale of 1-5 for the breed's tendancy to be open to strangers (Trait_Score) |
|Playfulness Level           |character | Placement on scale of 1-5 for the breed's tendancy to be playful (Trait_Score) |
|Watchdog/Protective Nature         |character | Placement on scale of 1-5 for the breed's "Watchdog/Protective Nature" (Trait_Score) |
|Adaptability Level         |character | Placement on scale of 1-5 for the breed's tendancy to be adaptable (Trait_Score) |
|Trainability Level        |character | Placement on scale of 1-5 for the breed's tendancy to be adaptable (Trait_Score) |
|Energy Level         |character | Placement on scale of 1-5 for the breed's "Energy Level" (Trait_Score) |
|Barking Level         |character | Placement on scale of 1-5 for the breed's "Barking Level" (Trait_Score) |
|Mental Stimulation Needs         |character | Placement on scale of 1-5 for the breed's "Mental Stimulation Needs" (Trait_Score) |

### `trait_description.csv`

|variable        |class     |description |
|:---------------|:---------|:-----------|
|Trait    |character | Dog Breed |
|Trait_1            |character | Value corresponding to `Trait` when `Trait_Score` = 1 |
|Trait_5            |character    | Value corresponding to `Trait` when `Trait_Score` = 5 |
|Description            |character | Long description of trait |

### `breed_rank_all.csv`

|variable        |class     |description |
|:---------------|:---------|:-----------|
|Breed    |character | Dog Breed |
|2013 Rank            |character | Popularity of breed based on AKC registration statistics in 2013 |
|2014 Rank            |character | Popularity of breed based on AKC registration statistics in 2014 |
|2015 Rank            |character | Popularity of breed based on AKC registration statistics in 2015 |
|2016 Rank            |character | Popularity of breed based on AKC registration statistics in 2016 |
|2017 Rank            |character | Popularity of breed based on AKC registration statistics in 2017 |
|2018 Rank            |character | Popularity of breed based on AKC registration statistics in 2018 |
|2019 Rank            |character | Popularity of breed based on AKC registration statistics in 2020 |
|2020 Rank            |character | Popularity of breed based on AKC registration statistics in 2019 |
|links            |character    | Link to the dog breed's AKC webpage |
|Image            |character    | Link to image of dog breed |

********************************************************

Scripts to retrieve the data: 
- [webscraping_script-1.Rmd](https://github.com/kkakey/dog_traits_AKC/blob/main/webscraping_script-1.Rmd)
- [webscraping_script-2.Rmd](https://github.com/kkakey/dog_traits_AKC/blob/main/webscraping_script-2.Rmd)

Last retrieved on Dec. 23, 2021

