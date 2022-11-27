# domestic-ASD-dataset-details

This page reports:
* In **Table 1**, a list of all the files that were discarded from the DESED and TUT Rare Sound Events Development datasets for the creation of the dataset described in Alessandro Ilic Mezza, Giulio Zanetti, Maximo Cobos, and Fabio Antonacci,"Zero-Shot Anomalous Sound Detection in Domestic Environments Using Large-Scale Pretrained Audio Pattern Recognition Models";
* In **Table 2**, a list of all the files that were used as registered events/anomalies to test our method.

File names are expressed in the format `ID_TAKE`, where `ID` corresponds to the Freesound ID of the original audio file and `TAKE` progressively enumerates the isolated events originating from the same file, starting from 0. Each `TAKE` corresponds to an individual event obtained from splitting the original sample, when such sample contains several events of the same class separated by silence or irrelevant data (e. g. a Freesound audio file may contain N separated events, and it will be split in N different audio files). For the TUT Rare Sound Events Development dataset (classes "Baby cry", "Glass break", and "Gunshot"), the timestamps of the isolated audioevents are annotated in the accompanied yaml meta-files, and the code provided by the author makes possible to split the original Freesound files into per-event audio files using such data. All the audio files provided in the DESED dataset (classes "Alarm bell ringing", "Dog", "Electric shaver/Toothbrush") already come as single-event audio files using the descibed `ID_TAKE` notation.

## Table 1
List of files picked as registered events/anomalies. The first file for every column was used to test the 1-shot case of every ASD system, while for the 3-shot case all of them were used.

| Baby cry   | Glass break   | Gunshot     | Alarm bell ringing   | Dog        | Electric shaver/Toothbrush   |
|------------|---------------|-------------|----------------------|------------|------------------------------|
| `271351_2` | `86568_9`     | `377786_8`  | `255193_0`           | `59513_5`  | `94298_1`                    |
| `244236_3` | `320126_2`    | `260600_10` | `151242_0`           | `4918_2`   | `328985_1`                   |
| `211527_3` | `257642_3`    | `255264_2`  | `13613_0`            | `348129_6` | `188364_1`                   |

## Table 2
List of files discarded during dataset creation. If `TAKE` is not specified, it means that all the isolated events generated from that Freesound ID have been discarded.

| Baby cry                                                                                                                                                                                                                                                                                                                                                                                                       | Glass break                                                                                                                                                                         | Gunshot                                                                                                                                                                                                                                                     | Alarm bell ringing                                                                                                                                                                                                                                                        | Dog                                                                                                                                                                                                                                                                                                                                                      | Electric shaver/Toothbrush                                                                                              |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------|
| `271352_0 `<br /> `271352_3 `<br /> `271352_4 `<br /> `271352_5 `<br /> `271352_10`<br /> `31527_0  `<br /> `31527_2  `<br /> `31529     `<br /> `31530     `<br /> `31531     `<br /> `31532     `<br /> `146925    `<br /> `175897    `<br /> `185575    `<br /> `211527_6 `<br /> `242119_0 `<br /> `244236_1 `<br /> `244236_2 `<br /> `271351_5 `<br /> `31527_1  `<br /> `31532_2  `<br /> | `360621_1`<br /> `362238   `<br /> `368342_0`<br /> `369987   `<br /> `57947_2 `<br /> `57971_0 `<br /> `57971_1 `<br /> `57971_2 `<br /> `270517_0`<br /> `327591_0`<br /> | `30185    `<br /> `127845   `<br /> `127846   `<br /> `163738_0`<br /> `204011_0`<br /> `248204_1`<br /> `249778_0`<br /> `257876   `<br /> `258203_0`<br /> `320135   `<br /> `332934_0`<br /> `332935   `<br /> `341221   `<br /> `343435_0`<br /> | `70102     `<br /> `233645_6 `<br /> `233645_14`<br /> `233645_16`<br /> `329896_20`<br /> `424946    `<br /> `20101     `<br /> `38229     `<br /> `54277     `<br /> `69185     `<br /> `79440     `<br /> `79633     `<br /> `79638     `<br /> `80341     `<br /> | `380156`<br /> `55154 `<br /> `84654 `<br /> `115357`<br /> `121891`<br /> `128023`<br /> `128036`<br /> `128040`<br /> `235876`<br /> `244469`<br /> `341090`<br /> `236011`<br /> `236052`<br /> `236054`<br /> `212128`<br /> `249303`<br /> `275069`<br /> `275070`<br /> `275071`<br /> `275072`<br /> `275565`<br /> `275566`<br /> `370919`<br /> | `51677 `<br /> `155512`<br /> `331161`<br /> `393536`<br /> `91516 `<br /> `91517 `<br /> `126392`<br /> `250011`<br /> |
