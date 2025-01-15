```markdown
# RSE_project_group13 Instructions

Below are the steps to run the code with our updates.

---

## 1. Download and Run the Code

1. **Download** the code to your local computer.  
2. **Open a terminal** and navigate (`cd`) to the repository directory.  
3. **Run** the following commands:
   ```bash
   ./services create
   ./services start
   ```
4. Wait for the services to start. Once you see:
   ```
   done
   ⏳ Waiting for Keyrock to be available

   done
   ```
   open your browser to [http://localhost:8000](http://localhost:8000).

---

## 2. Updating the Project Files

To add parts of our project (with a functioning frontend), follow these steps:

1. **Open the Docker dashboard** on your computer.  
2. **Open the fiware container**, then open the `fiware-tutorial` container.  
3. Navigate through the file system:
   - `opt` directory  
   - `tutorial` directory  

Inside this `tutorial` directory, **three files** must be replaced with the updated files from this code repository:

1. `devices.js` (in the `models` folder)  
2. `device.pug` (in the `views` folder)  
3. `device-monitor.pug` (in the `views` folder)

Then restart the containter in the docker desktop

### 2.1 How to Update Each File

1. Click the **Open File Editor** in the Docker container.  
2. **Delete** the existing file.  
3. **Copy and paste** the contents from the corresponding `updated_*.js` or `updated_*.pug` file in this repository.  

For example, replace `devices.js` with `updated_devices.js`. Do the same for `device.pug` and `device-monitor.pug`.

We have included the original files (named `og_...`) alongside the updated files (`updated_...`) to highlight our changes.

---

## 3. Viewing the Frontend and Logging In

Now you can view our frontend and devices at [http://localhost:3000](http://localhost:3000).  

To ensure that the IoT devices are running, open the **tutorial application** (`http://localhost:3000/`) in a new browser window.  
- **Log in** with the following credentials:  
  - **Email:** `bob-the-manager@test.com`  
  - **Password:** `test`  
- Once logged in, click on **device monitor**. Bob can switch on the lamp to obtain context data for the mashup.

---

## 4. Persisting the Changes

To keep the changes permanently, **commit the Docker container** after the file replacements are done. Otherwise, the changes may be lost if the container is rebuilt.

---

That’s it! You should now have the updated project running at [http://localhost:8000](http://localhost:8000).
```