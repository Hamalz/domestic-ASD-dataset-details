# domestic-ASD-dataset-details

This repository provide additional information on the dataset presented in
> [1] Alessandro Ilic Mezza, Giulio Zanetti, Maximo Cobos, and Fabio Antonacci, "Zero-Shot Anomalous Sound Detection in Domestic Environments Using Large-Scale Pretrained Audio Pattern Recognition Models," _unpublished_, 2022. 

The dataset contains sound events gathered from two different existing datasets. Acoustic anomalies are taken from the [TUT Rare Sound Events Development](https://zenodo.org/record/401395#.Y4UdDX3MKMo) dataset, and belong to three classes, i.e., “Baby cry,” “Glass break,” and “Gunshot.” As non-anomalous events, we select three classes from the Domestic Environment Sound Event Detection Dataset ([DESED](https://zenodo.org/record/6026841#.Y4UxjX3MKMo)), i.e., “Dog,” “Alarm bell ringing,” and “Electric shaver/Toothbrush.”

## TUT Rare Sound Events Development

The TUT Rare Sound Events Development dataset contains recordings gathered from [Freesound](https://freesound.org/) in the form of wav files, the name of which corresponds with their unique Freesound ID. We split the files using the processing function `freesound_files_into_event_wise_files` provided by the authors ([here](https://github.com/TUT-ARG/TUT_Rare_sound_events_mixture_synthesizer)), thus obtaining several wav files corresponding to isolated sound events.

In **Table 1.a**, we report a list of all the files that were used as registered anomalies to test the memory-based anomalous sound detection methods in [1].

In **Table 1.b**, we report a list of all the files that were discarded from the TUT Rare Sound Events Development dataset for the creation of the dataset described in [1].


### Table 1.a
| Baby cry       | Glass break       | Gunshot         |
|----------------|-------------------|-----------------|
| `271351_2.wav` | `86568_9.wav`     | `377786_8.wav`  |
| `244236_3.wav` | `320126_2.wav`    | `260600_10.wav` |
| `211527_3.wav` | `257642_3.wav`    | `255264_2.wav`  |

### Table 1.b
| Baby cry                                                                                                                                                                                                                                                                                                                                                                                                                                  | Glass break                                                                                                                                                                                               | Gunshot                                                                                                                                                                                                                                                                                |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `271352_0.wav.wav`<br /> `271352.wav.wav`<br /> `271352_4.wav`<br /> `271352_5.wav`<br /> `271352_10.wav`<br /> `31527_0.wav`<br /> `31527_2.wav`<br /> `31529.wav`<br /> `31530.wav`<br /> `31531.wav`<br /> `31532.wav`<br /> `146925.wav`<br /> `175897.wav`<br /> `185575.wav`<br /> `211527_6.wav`<br /> `242119_0.wav`<br /> `244236_1.wav`<br /> `244236_2.wav`<br /> `271351_5.wav`<br /> `31527_1.wav`<br /> `31532_2.wav`<br /> | `360621_1.wav`<br /> `362238.wav`<br /> `368342_0.wav`<br /> `369987.wav`<br /> `57947_2.wav`<br /> `57971_0.wav`<br /> `57971_1.wav`<br /> `57971_2.wav`<br /> `270517_0.wav`<br /> `327591_0.wav`<br /> | `30185.wav`<br /> `127845.wav`<br /> `127846.wav`<br /> `163738_0.wav`<br /> `204011_0.wav`<br /> `248204_1.wav`<br /> `249778_0.wav`<br /> `257876.wav`<br /> `258203_0.wav`<br /> `320135.wav`<br /> `332934_0.wav`<br /> `332935.wav`<br /> `341221.wav`<br /> `343435_0.wav`<br /> |

## DESED

We selected three classes of "foreground" events from the DESED dataset and we used the files as provided.

In **Table 2.a**, we report a list of all the files that were used as registered non-anomalous events to test the memory-based anomalous sound detection methods in [1].

In **Table 2.b**, we report a list of all the files that were discarded from the DESED dataset for the creation of the dataset described in [1].

### Table 2.a

| Alarm bell ringing       | Dog            | Electric shaver/Toothbrush       |
|--------------------------|----------------|----------------------------------|
| `255193_0.wav`           | `59513_5.wav`  | `94298_1.wav`                    |
| `151242_0.wav`           | `4918_2.wav`   | `328985_1.wav`                   |
| `13613_0.wav`            | `348129_6.wav` | `188364_1.wav`                   |

### Table 2.b

| Alarm bell ringing                                                                                                                                                                                                                                                           | Dog                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Electric shaver/Toothbrush                                                                                                                           |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| `70102.wav`<br /> `233645_6 .wav`<br /> `233645_14.wav`<br /> `233645_16.wav`<br /> `329896_20.wav`<br /> `424946.wav`<br /> `20101.wav`<br /> `38229.wav`<br /> `54277.wav`<br /> `69185.wav`<br /> `79440.wav`<br /> `79633.wav`<br /> `79638.wav`<br /> `80341.wav`<br /> | `380156.wav`<br /> `55154 .wav`<br /> `84654 .wav`<br /> `115357.wav`<br /> `121891.wav`<br /> `128023.wav`<br /> `128036.wav`<br /> `128040.wav`<br /> `235876.wav`<br /> `244469.wav`<br /> `341090.wav`<br /> `236011.wav`<br /> `236052.wav`<br /> `236054.wav`<br /> `212128.wav`<br /> `249303.wav`<br /> `275069.wav`<br /> `275070.wav`<br /> `275071.wav`<br /> `275072.wav`<br /> `275565.wav`<br /> `275566.wav`<br /> `370919.wav`<br /> | `51677.wav`<br /> `155512.wav`<br /> `331161.wav`<br /> `393536.wav`<br /> `91516.wav`<br /> `91517.wav`<br /> `126392.wav`<br /> `250011.wav`<br /> |

## CSV files

This repository also contains CSV files corresponding to the tables described above. The file `discarded_files.csv` specifies the files discarded in creating the dataset, whereas `examples.csv` specifies the files used as registered anomalies/events.
