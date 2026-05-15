<h2>Daily Task Report – Member 1</h2>

<table border="1" cellpadding="10" cellspacing="0">

  <tr>
    <th>Date</th>
    <th>Task Completed</th>
    <th>Description / Progress</th>
    <th>Challenges</th>
    <th>Next Step</th>
  </tr>

  <tr>
    <td>12 May 2026</td>
    <td>Data Exploration</td>
    <td>
      Loaded train_data.parquet and explored dataset structure.
      Checked Sample_ID counts and verified each sample has 100 rows.
    </td>
    <td>
      Understanding parquet file structure.
    </td>
    <td>
      Visualise sensor signals and investigate missing values.
    </td>
  </tr>

  <tr>
    <td>15 May 2026</td>
    <td>Feature Engineering</td>
    <td>
      Only the 14 sensor signal columns were used for feature extraction, while Sample_ID and Time_Step were excluded because they are identifiers and sequence markers rather than actual sensor measurements. A reusable feature extraction function was created to convert each Sample_ID, which originally consisted of 100 sequential rows of sensor readings, into a single machine learning feature vector. Several types of features were extracted from each signal, including statistical features such as mean, standard deviation, minimum, maximum, median, skewness, kurtosis, and interquartile range. Temporal features such as signal slope, zero crossings, and number of peaks were also computed to capture how the signals changed over time. In addition, Fast Fourier Transform (FFT) features were extracted to analyse frequency patterns within the movements, including FFT mean, FFT maximum, and dominant frequency. The extracted features were combined into structured training and testing feature tables, merged with the training labels, checked for missing values, and saved as X_train_features.parquet, X_test_features.parquet, and train_features_with_labels.parquet for use in the modelling and validation stage of the assignment.
    </td>
    <td>
  No challenges faced
    </td>
    <td>
      Saved files as  X_train_features.parquet, X_test_features.parquet, and train_features_with_labels.parquet
    </td>
  </tr>

 

</table>
