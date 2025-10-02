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
![Uploading Screenshot 2025-10-02 150444.png…]()

---

## 📸 Screenshot

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
