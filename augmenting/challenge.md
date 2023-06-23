# Develop a platform for accessing and augmenting climate datasets with other data sources

## Background

Many climate datasets exist [however these are not necessarily easy for researchers to use](https://wellcome.org/reports/combining-climate-and-health-data-challenges-and-opportunities-longitudinal-population). One difficulty is that climate data are found over many different spatiotemporal scales which means that most datasets are not immediately compatible with each other. This is especially true when considering how climate data can be used to augment health data, financial data, and other data sources. Data cleaning is the starting point of any analysis however for climate data even this can provide a barrier to entry, we want to remove this barrier.

## Challenge

Create a sophisticated data infrastructure platform for multiple data sources across differing spatiotemporal scales that includes Extract Transform
Load pipelines for loading different data types and for data augmentation. Your platform should be as flexible as possible and should provide generic pipelines for custom pre-processing. Your platform should enable storing and sharing pipelines (but should not force users to do so) and should allow users to upload their own data. As an example (and you do not need to do this as part of the challenge) your platform could enable workflows such as:

* Upload Electronic Health Record (EHR) data with hospital-level data measured on a daily scale to a local environment ensuring the data will not be shared further;
* Collapse the data to be on a monthly scale;
* Pull methane emission data from an online data source measured at a national level on an annual scale and then interpolate this to a monthly scale;
* Augment the EHR data with the methane data by using hospital look-up information to match hospital locations;
* Visualise the augmented data on the platform and perform basic analysis using a graphical interface;
* Download processed data for further analysis and save pipeline.

## Questions to answer in your presentation

1. How can your platform handle multiple types of data and how can users choose how data can be collapsed and interpolated? How will you trade-off user-choice against design decisions that favour optimal methods?
2. How would you visualise complex data across multiple spatiotemporal scales?
3. How can users search and access data and be informed about benefits and limitations (including possible biases) of data and data types across different scales?
