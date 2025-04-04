# 📘 Linguagens Formais e Autômatos

## 1️⃣ **Expressões Regulares**

- 🔹 **L1** = {w | w possui `aaa` como subpalavra}  
  📝 **Expressão regular:** `(a + b)*aaa(a + b)*`

- 🔹 **L2** = {w | o sufixo de w é `bb`}  
  📝 **Expressão regular:** `(a + b)*bb`

- 🔹 **L3** = {w | `bb` é subpalavra de w e `aaaa` é sufixo}  
  📝 **Expressão regular:** `(a + b)*bb(a + b)*aaaa`

- 🔹 **L4** = {w | w possui sufixo `aaa` ou prefixo `bb` ou w = ε}  
  📝 **Expressão regular:** `(a + b)*aaa + bb(a + b)* + ε`

- 🔹 **L5** = {w | w possui sufixo `ba` e prefixo `ab`}  
  📝 **Expressão regular:** `ab(a + b)*ba`

---

## 2️⃣ **Autômatos Finitos**

### ⚙️ i. Expressão Regular: `(b + ab)*`  
📷 ![image](https://github.com/user-attachments/assets/5f285be4-c70e-4df0-a05b-1118cd31231c)

### ⚙️ ii. Expressão Regular: `(a + ε)(b + ba)`  
📷 ![image](https://github.com/user-attachments/assets/0f65d3cf-34bf-4e44-97e4-149e8cd47e15)

### ⚙️ iii. Expressão Regular: `(ab + ba)*(aa + bb)`  
📷 ![image](https://github.com/user-attachments/assets/d2ba67eb-600a-4d9c-9ca9-90826d02254e)


### ⚙️ iv. Expressão Regular: `ab(abb* + baa*)*ba`  
📷 ![image](https://github.com/user-attachments/assets/61f682fd-fa48-46c2-865c-efe0b6c3847e)

### ⚙️ v. Expressão Regular: `(aa + b)*(a + bb)`  
📷 ![image](https://github.com/user-attachments/assets/36c58e5e-0c49-4af7-8858-6969f5f2014c)

### ⚙️ vi. Expressão Regular: `a*(aa + bb)`  
📷 ![image](https://github.com/user-attachments/assets/5ab3238d-28d8-494d-b97e-7fcfb8aa3564)

### ⚙️ vii. Expressão Regular: `b*ab*ab*`  
📷 ![image](https://github.com/user-attachments/assets/4f56c27c-f96f-4a57-a9f1-9c1815d94b46)

### ⚙️ viii. Expressão Regular: `(b + ab)*(ε + a)`  
📷 ![image](https://github.com/user-attachments/assets/c7c2fd2f-a3de-4f37-bd70-33f4acf2bfab)

### ⚙️ ix. Expressão Regular: `(aa + bb)*(ab)*`  
📷 ![image](https://github.com/user-attachments/assets/2bf29c58-6abc-47fc-af9f-7a1535485afa)

### ⚙️ x. Expressão Regular: `(ab + ba)*(aa + bb)*`  
📷 ![image](https://github.com/user-attachments/assets/c9cf40d4-9737-40c5-9df9-ccd7b19de898)

---

## 3️⃣ **Identificação das Linguagens Denotadas pelas Expressões Regulares**

- 🧠 **i.** `(aa + b)*(a + aa)`  
  🔍 Denota: Repete várias vezes "aa" e "b", e termina com "a" ou "aa".

- 🧠 **ii.** `(b + ab)*(ε + a)`  
  🔍 Denota: Repete várias vezes "b" e "ab", e termina com vazio ou "a".

- 🧠 **iii.** `(ab + ba)(b + a)* ba`  
  🔍 Denota: "ab" ou "ba" como prefixo, seguido de qualquer sequência de "a"s e "b"s, e termina com "ba".

- 🧠 **iv.** `(0 + 1)* 111 (0 + 1)* 111`  
  🔍 Denota: A sequência "111" aparece como subpalavra duas vezes (em qualquer lugar da palavra).

---

