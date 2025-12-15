

# 🎓 Digital Signal Processing Lab - TD-02

Solutions for Digital Signal Processing exercises on signal sampling and aliasing.

## 📚 Course Information
- **Institution**: ENSA-Tétouan, University Abdelmalek Essaadi (UAE)
- **Academic Year**: 2025-26
- **Subject**: Digital Signal Processing
- **Topic**: Sampling, Aliasing, and Signal Recovery

---

## 📝 Exercises Overview

### Exercise 1: Basic Signal Sampling
- **Signal**: `x(t) = 5*cos(2π*1000*t)`
- **Sampling Rate**: 8 kHz
- **Tasks**: Spectrum analysis of original and sampled signals

### Exercise 2: Multi-frequency Signal Processing
- **Signal**: `x(t) = 5*cos(2π*2000*t) + 3*cos(2π*3000*t)`
- **Sampling Rate**: 8 kHz
- **Tasks**: Recovery using ideal lowpass filter (4 kHz cutoff)

### Exercise 3: Aliasing Demonstration
- **Signal**: `x(t) = 5*cos(2π*2000*t) + cos(2π*5000*t)`
- **Sampling Rate**: 8 kHz
- **Tasks**: Analyze aliasing effects when frequency exceeds Nyquist

### Exercise 4: Complex Multi-component Analysis
- **Signal**: `x(t) = 1 + cos(2π*2000*t) + 2*cos(2π*4000*t) + 3*cos(2π*6000*t)`
- **Sampling Rate**: 8 kHz
- **Tasks**: Unilateral/bilateral spectra, aliasing identification, signal recovery

---

## 🚀 How to Use

### Prerequisites
```bash
pip install numpy matplotlib jupyter
```

### Running the Jupyter Notebook
```bash
jupyter notebook "PROJET TNS.ipynb"
```

Or run individual exercises as Python scripts (if you create separate `.py` files).

---

## 📊 Results Summary

| Exercise | Signal Frequencies | Sampling Rate | Aliasing? | Recovery |
|----------|-------------------|---------------|-----------|----------|
| 1 | 1 kHz | 8 kHz | ❌ No | ✅ Perfect |
| 2 | 2 kHz, 3 kHz | 8 kHz | ❌ No | ✅ Perfect |
| 3 | 2 kHz, 5 kHz | 8 kHz | ⚠️ Yes (5kHz→3kHz) | ❌ Corrupted |
| 4 | DC, 2-6 kHz | 8 kHz | ⚠️ Yes (6kHz→2kHz) | ❌ Corrupted |

---

## 🎯 Key Concepts Covered

### Nyquist-Shannon Sampling Theorem
- Minimum sampling rate: `fs ≥ 2 * fmax`
- Nyquist frequency: `fN = fs/2`

### Aliasing
- Occurs when: `f_signal > fs/2`
- Alias frequency: `f_alias = |f_signal - k*fs|`

### Signal Recovery
- Ideal lowpass filter reconstruction
- Cutoff frequency selection
- Limitations due to aliasing

---

## 🛠️ Technologies Used

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![NumPy](https://img.shields.io/badge/NumPy-1.21+-green.svg)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.4+-red.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)

---

## 📁 Repository Contents

- `PROJET TNS.ipynb` - Jupyter notebook with all exercises and solutions
- `sousou.pdf` - Original exercise sheet from ENSA
- `README.md` - This documentation file
- `.gitignore` - Python gitignore configuration

---

## 📈 What Each Exercise Demonstrates

Each exercise generates visualizations showing:
- ✅ Original signal spectrum (frequency domain)
- ✅ Sampled signal spectrum with replicas
- ✅ Recovered signal spectrum after filtering
- ✅ Aliasing effects (where applicable)
- ✅ Detailed mathematical analysis

---

## 👤 Author

**Markad Sultana**
- GitHub: [@markadsultana](https://github.com/markadsultana)
- Institution: ENSA-Tétouan
- Course: Digital Signal Processing (GSTR1)

---

## 📄 License

This project is available for educational purposes.

---

## 🤝 Contributing

This is an educational project. Suggestions and improvements are welcome:
1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

---

**Last Updated**: December 2024

---

*Developed as part of the Digital Signal Processing course at ENSA-Tétouan, University Abdelmalek Essaadi*
```

4. **Scroll down** and in the commit message box type:
```
   Update README with comprehensive documentation
```

5. **Click "Commit changes"**

### **3. Create a Requirements File**
1. Click **"Add file"** → **"Create new file"**
2. Name it: `requirements.txt`
3. Paste:
```
   numpy>=1.21.0
   matplotlib>=3.4.0
   jupyter>=1.0.0
