# React Native Problem-Solving Interview Questions & Answers

## 🔧 Top 10 Questions with Answers

---

### 1. [App crash debugging](ca://s?q=React_Native_app_crash_debugging)  
**Question:** Your app crashes only on Android 12 devices. How do you systematically debug and isolate the issue?  
**Answer:**  
- Check **logcat** for crash traces.  
- Verify **permissions** (Android 12 introduced new Bluetooth/notification permissions).  
- Test with **different device models** to isolate OEM-specific issues.  
- Use **Gradle build variants** to reproduce and patch.  

---

### 2. [Slow startup time](ca://s?q=React_Native_slow_startup_time)  
**Question:** Users complain the app takes too long to launch. What steps would you take to profile and reduce startup time?  
**Answer:**  
- Use **Systrace/Flipper** to profile startup.  
- Enable **Hermes engine** for faster JS execution.  
- Apply **code splitting** and lazy loading.  
- Reduce **bundle size** by removing unused libraries.  

---

### 3. [Network request failure](ca://s?q=React_Native_network_request_failure)  
**Question:** API calls intermittently fail on poor connections. How would you implement retry logic and offline caching?  
**Answer:**  
- Use **Axios interceptors** for retry logic with exponential backoff.  
- Implement **offline-first caching** with AsyncStorage/MMKV.  
- Queue requests and sync when connection restores.  

---

### 4. [UI lag on scroll](ca://s?q=React_Native_UI_scroll_lag)  
**Question:** A FlatList scroll stutters when rendering images. How do you optimize list rendering and image loading?  
**Answer:**  
- Use **`getItemLayout`** and **`keyExtractor`** for efficient rendering.  
- Memoize row components with **React.memo**.  
- Use **react-native-fast-image** for caching.  
- Avoid inline functions in renderItem.  

---

### 5. [State management bug](ca://s?q=React_Native_state_management_bug)  
**Question:** A Redux store update doesn’t reflect in the UI. How do you debug and fix state synchronization issues?  
**Answer:**  
- Check if **reducers return new state objects** (immutability).  
- Verify **mapStateToProps/useSelector** is correctly subscribed.  
- Ensure **middleware** isn’t swallowing actions.  
- Use Redux DevTools to trace dispatched actions.  

---

### 6. [Push notification issue](ca://s?q=React_Native_push_notification_issue)  
**Question:** Notifications arrive but don’t open the correct screen. How do you debug deep linking and navigation integration?  
**Answer:**  
- Verify **notification payload** includes correct deep link.  
- Configure **React Navigation linking** properly.  
- Test with **cold start vs foreground state**.  
- Use **Firebase console** to simulate payloads.  

---

### 7. [Memory leak detection](ca://s?q=React_Native_memory_leak_detection)  
**Question:** The app’s memory usage keeps growing after navigation. How do you detect and fix memory leaks?  
**Answer:**  
- Use **Xcode Instruments/Android Profiler** to track leaks.  
- Ensure **event listeners** are removed in `useEffect` cleanup.  
- Avoid retaining references in closures.  
- Profile navigation stack for unmounted screens.  

---

### 8. [Gesture conflict](ca://s?q=React_Native_gesture_conflict)  
**Question:** A swipe gesture conflicts with a scroll view. How do you resolve gesture handler conflicts?  
**Answer:**  
- Use **react-native-gesture-handler** with proper priority.  
- Apply **`waitFor`** or **`simultaneousHandlers`** props.  
- Test gestures separately to isolate conflicts.  

---

### 9. [Image upload failure](ca://s?q=React_Native_image_upload_failure)  
**Question:** Large image uploads fail on mobile networks. How do you optimize uploads with compression and chunking?  
**Answer:**  
- Compress images using **react-native-image-resizer**.  
- Implement **chunked uploads** for large files.  
- Use **background upload tasks** for reliability.  
- Provide user feedback with progress bars.  

---

### 10. [OTA update rollback](ca://s?q=React_Native_OTA_update_rollback)  
**Question:** An over-the-air update breaks the app for some users. How do you design a safe rollback strategy?  
**Answer:**  
- Use **CodePush staged rollout** to limit exposure.  
- Implement **rollback triggers** if crash rate spikes.  
- Maintain **version compatibility checks**.  
- Always keep a **stable fallback build** in the app store.  

---

## 📊 Snapshot Table

| **[Problem](ca://s?q=React_Native_problem_solving)** | **Root Cause** | **Solution Approach** |
|----------------|-------------|----------------|
| App crash | OS-specific bug | Logs, permissions, OEM testing |
| Slow startup | Heavy bundle | Hermes, lazy loading, code splitting |
| Network failure | Poor connectivity | Retry logic, offline cache |
| UI lag | Excessive re-renders | Memoization, fast-image |
| Memory leak | Unreleased listeners | Profiling, cleanup in `useEffect` |

---

## 🎯 Usage
This file can be used as:
- A **study guide** for React Native interviews  
- A **mock interview script** for practice  
- A **team exercise** to discuss debugging strategies
