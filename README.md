# Duplicate Analysis of AcousticBrainz Submissions

There are many duplicate submissions in AcousticBrainz, files that represent the same music recording (and have the same MBID) but were submitted by many people. These files could be from different sources (e.g. different CDs issues, a remastered CD, a recorded vinyl, a radio edit) and could be encoded using different formats (MP3, Flac, AAC). A dataset of only songs with more than 1 submission has been made available [here](http://www.dtic.upf.edu/~aporter/amplab/).

Also, there are some submissions in AcousticBrainz that have been incorrectly labeled. That is, the contents of the file which was analysed is not the file which the MBID label indicates. The goal of this task is to find which submissions in the provided dataset are mislabeled. In this context, it will be helpful to know which of the submissions were duplicates for sure. Hence, I would like to propose an analysis approach which will tell us most certain duplicates and most certain non-duplicates.

The descriptors - 'length', 'bpm', 'average loudness', 'onset rate', 'key_key', 'key_scale', 'replaygain' and 'tuning frequency' have been considered. We then rejected some of these descriptors by estimating how useful they are.

The dataset for this task has been made available as an archive of json files, in the format that AcousticBrainz uses to store the data. Since, I did not need all of the data included in these files, I reduced the data to just the necessary values, and then worked with that data. I then looped through each of the files, extracted each of these features, and stored them in a CSV file.

#### A submission by Venkatesh Shenoy Kadandale, SMC Master Student 2017-18 as a part of Audio and Music Processing Lab Course
