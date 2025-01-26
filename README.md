# **TOPSIS Package**  
_A Python package for decision-making using the TOPSIS method._  

---

## **What is TOPSIS?**  
The **Technique for Order Preference by Similarity to Ideal Solution (TOPSIS)** is a multi-criteria decision analysis method.  
It ranks alternatives based on their closeness to the ideal solution and farthest from the worst solution, making it an excellent tool for decision-making problems.  

---

## **Features**  
- Simple and efficient implementation of the TOPSIS algorithm.  
- Accepts a decision matrix via a CSV file.  
- Supports customizable weights and impacts for criteria.  
- Outputs the TOPSIS scores and ranks into an easy-to-read CSV file.  

---

## **Installation**  
You can install the package from PyPI using:  

```bash
pip install 102217186-abhaijeet-topsis==1.0.0
```

---

## **How to Use**  

### **Run the Package**  

You can run the TOPSIS package directly from the command line using:  

```bash
python -m 102217186_abhaijeet_topsis <input_file> <weights> <impacts> <output_file>
```

### **Parameters**  
- `<input_file>`: Path to the CSV file containing the decision matrix.  
- `<weights>`: Comma-separated weights for each criterion (e.g., `0.2,0.1,0.43,0.3`).  
- `<impacts>`: Comma-separated impacts for each criterion (e.g., `+,+,-,-`, where `+` indicates a benefit criterion and `-` indicates a cost criterion).  
- `<output_file>`: Path to the output CSV file where the results will be saved.  

---

## **Example Usage**  

### Input CSV (`input.csv`)  
```csv
c:\Users\CGDXK\Pictures\Screenshots\input.png
```  

### Command  
```bash
python -m 102217186_abhaijeet_topsis input.csv "0.2,0.1,0.4,0.3" "+,+,-,+"
output.csv
```

### Output CSV (`output.csv`)  
```csv
ID,Criteria1,Criteria2,Criteria3,Criteria4,TOPSIS Score,Rank
A,250,16,12,5,0.7722,2
B,200,16,8,3,0.2251,4
C,300,32,16,7,0.8371,1
D,275,40,20,10,0.4213,3
```  

---

## **How It Works**  
1. **Normalization**: The decision matrix is normalized to bring all criteria onto a comparable scale.  
2. **Weighting**: Each criterion is multiplied by its corresponding weight.  
3. **Ideal Solutions**: Calculates the ideal best and worst solutions based on the impacts.  
4. **Distance Calculation**: Computes the distance of each alternative from the ideal best and worst solutions.  
5. **Ranking**: Scores and ranks alternatives based on their relative closeness to the ideal solution.  

---

## **License**  
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.  

---

## **Support**  
If you encounter any issues or have questions, feel free to open an issue on [GitHub](https://github.com/yourusername/102217186-abhaijeet-topsis).  

---

This README file is now clean, structured, and visually appealing while providing all necessary information for the user. Let me know if you'd like any further changes!