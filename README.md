<p align="center">
  <h2><strong>Brain Computer Interface Foundation Model Benchmark</strong></h2>
</p>

![Neurosity EEG Dataset](https://i.imgur.com/CUZb72p.png)

Welcome to the Neurosity EEG Dataset repository, a comprehensive and curated compilation of brain-computer interface (BCI) data meticulously collected through the advanced Neurosity Crown 3 device. This dataset is designed to foster research and development in the fields of neuroscience, cognitive science, machine learning, and beyond. By providing high-quality, preprocessed EEG signals, we aim to support and accelerate innovations in brain-computer interface technologies and the understanding of neural dynamics.

## Dataset Overview
The Neurosity EEG Dataset comprises 133 individual BCI sessions, aggregating a refined selection from over ten million rows of raw data captured by the Neurosity Crown 3 EEG device. The dataset is formatted to support both academic researchers and technology developers with an interest in EEG and BCI applications.

### Key Features:
- Total Sessions: 133
- Total Data Points: 10,983,584 rows (cleaned and aggregated)
- Channels: 8 (CP3, C3, F5, PO3, PO4, F6, C4, CP4)
- Device Information:
    - Nickname: Crown-0DB
    - Manufacturer: Neurosity, Inc
    - Model: Crown 3
- Sampling Rate: 256 Hz

## Data Access
This dataset is stored in CSV format for easy use and accessibility. The data is organized by session, with each session's id marking it apart.

### Downloading the Data
The data can be accessed and downloaded through this repository. To clone the repository and fetch the dataset, use the following Git command:


```
git clone https://github.com/JeremyNixon/neurosity
cd neurosity
```

and then download the data zip file from this Drive url:

```
https://drive.google.com/file/d/1V6MTCZU0LJPs3xa1E0HYnN0syWgVsOKU/view?usp=sharing
```

## Data Structure
Each data file corresponds to a single EEG session and includes the following columns:

- <b>Timestamp</b>: Unix timestamp in milliseconds
- CP3, C3, F5, PO3, PO4, F6, C4, CP4: EEG data from the respective channels

## Usage Examples
Here are some basic examples of how to load and visualize the EEG data using Python:

### Loading Data
```
import pandas as pd

# Load a single session file
data = pd.read_csv('combined_dataset.csv')
print(data.head())
```

### Basic Plotting
```
import matplotlib.pyplot as plt

# Plot the EEG data for channel CP3
plt.figure(figsize=(12, 6))
plt.plot(data['Timestamp'], data['CP3'], label='CP3')
plt.title('EEG Data for Channel CP3')
plt.xlabel('Timestamp')
plt.ylabel('Amplitude')
plt.legend()
plt.show()
```

## Contributing
Contributions to this dataset are welcome. Whether it be in the form of additional data, error corrections, usage examples, or even analysis techniques, please feel free to fork this repository, make your changes, and submit a pull request.

## Citation
If you use the Neurosity EEG Dataset in your research, please cite it using the following BibTeX entry:
```
@misc{neurosity_eeg_dataset,
  title={Neurosity EEG Dataset},
  author={Nixon, Jeremy and Keller, AJ},
  year={2024},
  url={https://github.com/JeremyNixon/neurosity}
}
```

## License
This dataset is made available under the MIT License. For more detailed licensing information, please see the LICENSE.md file in this repository.

## Contact
For any queries regarding the dataset, please contact jeremy@omniscience.tech.

We hope that this dataset serves as a valuable resource for your research and development efforts in the exciting field of brain-computer interfaces. Happy exploring!