## Autonomous Magnetic Resonance Imaging (AMRI)

👉 [AMRI concept video][amri-concept-video]

Autonomous Magnetic Resonance Imaging, or AMRI, is meant to operate end-to-end.
What this means is that, AMRI should intelligently acquire, reconstruct and
visualize MR data.

We also introduce AMRI-Scanner as an Online Service (AMRI-SOS). AMRI-SOS is a free to use online service. Check out the [`amri-sos`][amri-sos] branch to learn more, or fill out this [form][amri-sos-form] to request AMRI-SOS scans.

### Why AMRI?
Globally, there are **4.6 MRI scanners per 1,000,000** people. In comparison, there are 36.72 per 1,000,000 in the United States [[1]](#references)[[2]](#references), and the **low-income countries have 0.1 per 1,000,000**. Annual Healthcare spending in the US is 700 billion USD. Of this **125 – 200 billion USD** (at least) is accounted for by diagnostic imaging [[3]](#references). Autonomous scanners can play a major role in tackling the challenges of delivering MR to a larger population with low-incomes. [[4]](#references).

### And what is MR Value?
MR value can be defined to the patient as the ratio of actionable diagnostic information to the costs or time incurred. A simplified and technically relevant definition of MR value is: ratio of contrast-to-noise ratio (CNR) to the total scanner (table) time.

### MRI scanner as an Intelligent Physical System (IPS)
AMRI is capable of transforming a conventional MR system into an IPS that can be characterised by the following capabilities:
- Cognizant
- Taskable
- Adaptive
- Ethical
- Reflective (Reuse, Retain, Revise)

The above capabilities would deliver an IPS that is knowledge-rich, and capable of long-term autonomy with minimal human intervention and supervision.

### Utilization of file standards
AMRI can be easily built, rebuilt and deployed as it leverages 4 existing file standards and introduces 1 new file standard. These file standards are:
- EMR file standard for subject information encryption
- Situation report (Sitrep) file standard for sampling MR system state (introduced in this work)
- Pulseq [[5, 6, 7]](#references) file standard for multi-vendor pulse sequence programming
- ISMRMRD file standard for acquired raw data
- DICOM file standard for reconstructed image data

### Self administered MR
AMRI can also enable self administered MR scanning with the inclusion of MR-safe A/V accessories.

  ![amri_self_admin](https://github.com/imr-framework/amri/blob/amri/amri_self_admin.png)

### Video demos
YouTube demos can be found here:
- Invivo experiment, [link][invivo-exp-1]
- Phantom experiment, [link][invivo-exp-2]

### Dependencies
google-cloud-speech
google-cloud-texttospeech
keras
numpy
Pillow
pyaudio
pyautogui
pygame
pandas
pydrive
pypulseq
scipy
tensorflow
tqdm

#### AMRI - Scanner as an Online Service (AMRI-SOS)
👉 [AMRI-SOS form][amri-sos-form] 👈

AMRI-SOS enables students and researchers with limited access to MRI hardware to leverage AMRI to run custom pulse sequences designed on the Pulseq [[5, 6, 7]](#references) framework. If you want to run your scans on a Siemens Prisma 3T, fill out this [form][amri-sos-form].

### References
[1] Atlas of MS 2013, https://www.msif.org/wp-content/uploads/2014/09/Atlas-of-MS.pdf

[2] Geethanath S, Vaughan Jr JT. Accessible magnetic resonance imaging: A review. Journal of Magnetic Resonance Imaging. 2019 Jan 14.

[3] Kelley, Robert. "Where can $700 billion in waste be cut annually from the US healthcare system." Ann Arbor, MI: Thomson Reuters 24 (2009).

[4] Wang, Ge, et al. "Image Reconstruction is a New Frontier of Machine Learning." IEEE transactions on medical imaging 37.6 (2018): 1289-1296.

[5] [Ravi, Keerthi Sravan, et al. "Pulseq-Graphical Programming Interface: Open source visual environment for prototyping pulse sequences and integrated magnetic resonance imaging algorithm development." Magnetic resonance imaging 52 (2018): 9-15.](https://www.sciencedirect.com/science/article/pii/S0730725X1830033X)

[6] Ravi, Keerthi, Sairam Geethanath, and John Vaughan. "PyPulseq: A Python Package for MRI Pulse Sequence Design." Journal of Open Source Software 4.42 (2019): 1725.

[7] [Layton, Kelvin J., et al. "Pulseq: A rapid and hardware‐independent pulse sequence prototyping framework." Magnetic resonance in medicine 77.4 (2017): 1544-1552.](https://onlinelibrary.wiley.com/doi/abs/10.1002/mrm.26235)

[amri-concept-video]: https://www.youtube.com/watch?v=2XroYwUxzD4
[amri-sos-form]: https://goo.gl/forms/1FpGeH7S9SJbaBP53
[invivo-exp-1]: https://youtu.be/ccKxyWZLjto
[inivo-exp-2]: https://youtu.be/ZToRLwXQW1A
[amri-sos]: https://github.com/imr-framework/amri/tree/amri-sos
