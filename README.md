# Deepfake Audio Detection

## Introduction
Deepfake audio detection involves identifying artificially generated or manipulated voice recordings. This can be achieved using machine learning models trained on real and synthetic speech datasets.

## Dataset
Common datasets for deepfake audio detection include:
- [DEEP-VOICE](https://www.kaggle.com/datasets/birdy654/deep-voice-deepfake-voice-recognition/data) (The Dataset used for this project)
- **ASVspoof** (Automatic Speaker Verification Spoofing)
- **LA (Logical Access) and PA (Physical Access) datasets**
- **WaveFake**

## Preprocessing Steps
1. Convert audio files to a uniform format (e.g., WAV, 16kHz, mono).
2. Extract features such as:
   - Mel-Frequency Cepstral Coefficients (MFCCs)
   - Spectrograms (Mel, STFT, CQT)
   - Raw waveform embeddings (using Wav2Vec2, OpenL3, etc.)

## Model Architectures
Popular deep learning models for deepfake audio detection:
- **CNN (Convolutional Neural Networks)**: Used on spectrograms.
- **LSTM (Long Short-Term Memory Networks)**: Works well with sequential data.
- **Fusion Models**: Combination of CNNs and RNNs for better performance.

## Training & Evaluation
1. **Train the model** on a labeled dataset of real and fake audio.
2. **Loss function**: Binary Cross-Entropy (BCE) for classification.
3. **Evaluation Metrics**:
   - Accuracy
   - Precision, Recall, and F1-Score
   - Equal Error Rate (EER)
   - Area Under Curve (AUC-ROC)



## Challenges
- Low-quality datasets can introduce bias.
- New deepfake generation techniques evolve rapidly.
- Real-time detection requires optimized models.

## Future Work
- Improve model generalization with adversarial training.
- Use self-supervised learning to reduce labeled data dependency.
- Combine multimodal approaches (audio + lip-sync detection).
- Deployment (Improvement)
  - API-based: Deploy using Flask/FastAPI.
  - Edge AI: Optimize for mobile/embedded devices.
  - Real-time detection: Integrate with streaming services.

## License
- [MIT License](./LICENSE) 

## References

1. H. Purwins, B. Li, T. Virtanen, J. Schlüter, S. Y. Chang and T. Sainath, "Deep learning for audio signal processing", IEEE Journal of Selected Topics in Signal Processing, vol. 13, no. 2, pp. 206-219, 2019.
2. D. Xie, L. Zhang and L. Bai, "Deep learning in visual computing and signal processing", Applied Computational Intelligence and Soft Computing, 2017.
3. A. B. Nassif, I. Shahin, I. Attili, M. Azzeh and K. Shaalan, "Speech recognition using deep neural networks: A systematic review", IEEE access, vol. 7, pp. 19143-19165, 2019.
4. A. M. Almars, "Deepfakes detection techniques using deep learning: a survey", Journal of Computer and Communications, vol. 9, no. 5, pp. 20-35, 2021.
5. M. V. Subbarao, A. K. Padavala and K. D. Harika, "Performance Analysis of Speech Command Recognition Using Support Vector Machine Classifiers" in Communication and Control for Robotic Systems, Singapore:Springer, pp. 313-325, 2022.
6. B. T. Balamurali, K. E. Lin, S. Lui, J. M. Chen and D. Herremans, "Toward robust audio spoofing detection: A detailed comparison of traditional and learned features", IEEE Access, vol. 7, pp. 84229-84241, 2019.
7. Ivan Perov, Daiheng Gao, Nikolay Chervoniy, Kunlin Liu, Sugasa Marangonda, Chris Ume, Mr Dpfks, Facenheim Carl Shift, RP Luis, Jian Jiang et al., "Deepfacelab: A simple flexible and extensible face swapping framework", arXiv preprint.
8. Porter Jon, "Another convincing deepfake app goes viral prompting immediate privacy backlash", The Verge. Archived from the original on 3 September 2019, November 2019.
9. K. Fagan, A viral video that appeared to show obama calling trump a ‘dips’ shows a disturbing new trend called ‘deep fakes’, 2018.
10. D. Guera and E. J. Delp, "Deepfake Video Detection Using Recurrent Neural Networks", 2018 15th IEEE International Conference on Advanced Video and Signal Based Surveillance (A VSS), pp. 1-6, 2018.
11. J. Fei, Z. Xia, P. Yu et al., "Exposing AI-generated videos with motion magnification", Multimed Tools Appl, 2020, [online] Available: https://doi.org/10.1007/s11042-020-09147-3.
12. N. S. Ivanov, A. V. Arzhskov and V. G. Ivanenko, "Combining Deep Learning and Super-Resolution Algorithms for Deep Fake Detection", 2020 IEEE Conference of Russian Young Researchers in Electrical and Electronic Engineering (EIConRus), pp. 326-328, 2020.
