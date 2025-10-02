# Task 7: Monitor System Resources Using Netdata

## 📌 Objective

Install **Netdata** and visualize system and application performance metrics using Docker.

---

## 🛠 Tools Used

* Docker
* Netdata (Official Docker Image)

---

## ⚙️ Steps Followed

1. **Pulled and ran Netdata container:**

   ```bash
   docker run -d --name=netdata -p 19999:19999 --cap-add SYS_PTRACE --security-opt apparmor=unconfined netdata/netdata
   ```

2. **Verified container:**

   ```bash
   docker ps
   ```

3. **Accessed dashboard:**
   

4. **Monitored resources:**

   * CPU usage
   * Memory usage
   * Disk activity
   * Docker containers
   * Alerts and health checks

5. **Captured screenshot** of running dashboard.
<img width="1106" height="969" alt="Screenshot 2025-10-02 150444" src="https://github.com/user-attachments/assets/efec8bd4-3381-40b1-8485-0bdce262ca3f" />
<img width="1585" height="616" alt="Screenshot 2025-10-02 232908" src="https://github.com/user-attachments/assets/e210b06f-6087-46ab-ba41-47cef74347d4" />

---<img width="1854" height="962" alt="Screenshot 2025-10-02 232722" src="https://github.com/user-attachments/assets/eb586b1f-0786-4950-b524-33c491d4a20d" />

<img width="1829" height="965" alt="Screenshot 2025-10-02 232702" src="https://github.com/user-attachments/assets/1658d9d3-f20c-436d-81e0-21c069447582" />
<img width="1864" height="956" alt="Screenshot 2025-10-02 232649" src="https://github.com/user-attachments/assets/27a600dc-da5e-4775-a6b2-29a95a6a5a90" />

<img width="1852" height="949" alt="Screenshot 2025-10-02 232633" src="https://github.com/user-attachments/assets/b5f79443-30f0-46c1-932f-d9c0e93b0976" />
<img width="1858" height="926" alt="Screenshot 2025-10-02 232621" src="https://github.com/user-attachments/assets/cb16f77c-fe52-4d13-ac06-097a3d87f04a" />

<img width="1850" height="971" alt="Screenshot 2025-10-02 232607" src="https://github.com/user-attachments/assets/7067d823-529c-41fa-9342-3d1af809a4be" />
<img width="1834" height="898" alt="Screenshot 2025-10-02 232548" src="https://github.com/user-attachments/assets/9ca67e3d-87d2-4401-a037-436f96fe7ab8" />

## 📸 Screenshot ![Uploading Screenshot 2025-10-02 232649.png…]()

![Uploading Screenshot 2025-10-02 150444.png…]()

![Netdata Dashboard](./screenshot.png)

---

## 📖 Key Learnings

* Netdata provides **real-time metrics** with very low overhead.
* It is easier to set up compared to Prometheus but more focused on visualization.
* Useful KPIs: CPU, memory, disk usage, container stats, and system alerts.

---

## 🚀 How to Reproduce

1. Install Docker
2. Run the Netdata container (command above)
3. Visit `http://localhost:19999` in browser

---

## ✅ Outcome

Successfully set up Netdata for real-time monitoring of system and app resources.
