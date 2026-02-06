# R3IO: Rotational RCS-Based Filtering 4D Radar-Inertial Odometry
**R3IO** is a robust state estimation framework leveraging a rotating 4D millimeter-wave radar. By employing a custom rotating mechanism to achieve omnidirectional perception, combined with an RCS-based filtering module and a weighted tightly-coupled IEKF fusion scheme, our system achieves superior localization accuracy and robustness, particularly in feature-sparse and degenerated environment.

![image](/docs/traj.png)
## ✨ Key Features
* **🔄 Omnidirectional Perception:** Utilizes a rotating platform with encoder-based motion compensation to overcome the limited FOV of standard 4D radars.
* **🎯 Robust Noise Filtering:** Implements a polar voxel filter based on **RCS** and **Elevation Uncertainty** to suppress multipath noise and preserve stable landmarks.
* **🔗 Weighted Tightly-Coupled Fusion:** A rigorous IEKF framework that fuses IMU propagation with RCS-weighted geometric and Doppler velocity residuals.
* **🌲 Sparse Scene Adaptability:** Demonstrates high robustness in unstructured environments, significantly outperforming fixed-view radar odometry methods.

## 📂 Dataset

We provide the **self-collected datasets** used in the paper to facilitate reproduction and further research. The datasets cover diverse scenarios including structured urban roads and unstructured open areas.

### Dataset Details
| Sequence | Duration | Length | Scene Type | Key Challenges |
| :--- | :--- | :--- | :--- | :--- |
| **Seq Road** | 291s | 367m | Structured Campus Roadway / Urban | Long Straight Road & Curb Extraction |
| **Seq Library** | 112s | 143m | Structured Campus Roadway / Dynamic | Continuous Curves & Curb Extraction |
| **Seq Square** | 370s | 501m | Highly Dynamic Campus / Dynamic | High Interference from Dynamic Objects |
| **Seq Court** | 105s | 149m | Open Basketball Court | Sparse Geometric Features & Partial Degeneracy |
| **Seq Lakeside** | 179s | 193m | Lakeside Path | Unstructured Environments & Degenerate Environments |
| **Seq Lake1** | 350s | 249m | Lake | Single-sided Featureless & Water Surface Multipath |
| **Seq Lake2** | 170s | 109m | Lake | Featureless Ahead & Water Surface Multipath |

### Download
Please download the rosbag files from the links below.

* **Google Drive:** [Our sell-collected rosbags](https://drive.google.com/drive/folders/158hGGi4lv38lCUhJOMhXyzGtz7HA4X7Q?usp=drive_link)

## 🔨 Code
The code is currently being organized and will be released soon.
