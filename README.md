# AWS-Assignments

## 📘 **Assignment 1: Convert `.pem` to `.ppk` (PuTTY-Compatible Private Key)**

### ✅ Objective:

Convert AWS PEM private key to PPK using terminal or PuTTYgen (for Windows).

### 🔧 Instructions:

### 💻 **Linux/macOS (Terminal - using `puttygen`):**

1. Install `putty-tools`:

   ```bash
   sudo apt install putty-tools  # Ubuntu/Debian
   sudo yum install putty        # Amazon Linux/CentOS/RHEL
   ```
2. Convert `.pem` to `.ppk`:

   ```bash
   puttygen my-key.pem -o my-key.ppk
   ```

### 🪟 **Windows (Using PuTTYgen):**

1. Download [PuTTYgen](https://www.puttygen.com/)
2. Open PuTTYgen → Load your `.pem` file → Save as `.ppk`.

---

## 📘 **Assignment 2: EC2 - Amazon Linux SSH Access via PuTTY**

### ✅ Objective:

Launch, connect, stop, and terminate an Amazon Linux EC2 instance using `.ppk` via PuTTY.

### 🔧 Steps:

1. **Launch Amazon Linux EC2**:

   * Type: `Amazon Linux 2023`
   * Key Pair: Use your key (`.pem`)
   * Security Group: Allow inbound SSH (port 22)
2. **Convert `.pem` to `.ppk`** (Refer Assignment 1)
3. **Open PuTTY**:

   * Host Name: `ec2-user@<Public-IP>`
   * SSH → Auth → Browse `.ppk`
4. **Connect**
5. **Stop & Start the Instance**
6. **Terminate the Instance**

---

## 📘 **Assignment 3: EC2 - Ubuntu SSH Access via PuTTY**

### ✅ Objective:

Repeat same steps as above, but with **Ubuntu** instance.

### 🧪 Steps:

1. Launch Ubuntu EC2 (`ubuntu 22.04`)
2. Security group → Allow port 22
3. SSH via PuTTY

   * Username: `ubuntu`
4. Stop & Terminate the instance.

---

## 📘 **Assignment 4: EC2 - Red Hat SSH Access via PuTTY**

### ✅ Objective:

Practice connecting to a **Red Hat Enterprise Linux (RHEL)** EC2 instance.

### 🧪 Steps:

1. Launch RHEL EC2 (e.g., RHEL 9)
2. Convert PEM to PPK
3. SSH via PuTTY

   * Username: `ec2-user`
4. Stop & Terminate

---

## 📘 **Assignment 5: EC2 - SUSE Linux SSH Access via PuTTY**

### ✅ Objective:

Launch and manage a **SUSE Linux** EC2 instance and connect via PuTTY.

### 🧪 Steps:

1. Launch **SUSE Linux Enterprise Server (SLES)**
2. Allow SSH in Security Group
3. SSH via PuTTY

   * Username: `ec2-user`
4. Stop & Terminate

---

## 📌 Notes:

* Replace `<Public-IP>` with your EC2 instance's current public IP.
* Always select correct **username** for the Linux distro:

  | Distro       | SSH Username |
  | ------------ | ------------ |
  | Amazon Linux | `ec2-user`   |
  | Ubuntu       | `ubuntu`     |
  | Red Hat      | `ec2-user`   |
  | SUSE         | `ec2-user`   |
