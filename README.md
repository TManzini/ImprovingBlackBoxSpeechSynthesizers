# Towards Improving The Intelligibility of Black Box Speech Synthesizers In Noise

This repository contains the dataset that was collected in conjunction with the publication "[Towards Improving The Intelligibility of Black Box Speech Synthesizers In Noise](https://www.nzini.com/data/papers/Towards%20Improving%20Intelligibility%20of%20Black%20Box%20Speech%20Synthesizers%20in%20Noise.pdf)". The dataset itself contains 1440 transcriptions of syntheic speech synthesizers under synthetic noise conditions to measure the errors that listeners make.

The dataset was collected with s from mechanical turk and the Carnegie Mellon University [TestVox](http://www.festvox.org/) test kit. 

## Dataset Shape
The dataset is contained in the file "[IBBSS_dataset.csv](https://github.com/TManzini/ImprovingBlackBoxSpeechSynthesizers/blob/master/IBBSS_data.csv)" here in the repository.

Each transcription contains the following information. 
* A unique ID that represents the listener that transcribed this example.
* A number which indicates which sound file this transcription this was for, for a given listener. (0 is the first sound file a listener heard, 1 is the second, etc.)
* The transcription that the listener entered. (An empty string if the listener indicates the listener did not understand any content from the synthesizer)
* The ground truth text which was provided to the synethizer.
* The standard deviation of the random noise that was added to the synthesized speech. 
* The frequency that was used as a threshold for a low pass filter that was applied to the synthesized speech. 
* The frequency that was used as a threshold for a high pass filter that was applied to the synthesized speech. 
* The name of the synthesizer that was used (Flite, E-Speak, Google). 
* The file type that was used for the experiment.

## Citation
If you use this dataset in your research please use the following citation.
~~~~ 
@inproceedings{manzini2018towards,
  title={Towards Improving Intelligibility of Black-Box Speech Synthesizers in Noise},
  author={Manzini, Thomas and Black, Alan},
  booktitle={International Conference on Speech and Computer},
  pages={367--376},
  year={2018},
  organization={Springer}
}
~~~~ 
