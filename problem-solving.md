# React Native Problem-Solving Interview Questions

## 🔧 Top 10 Questions

1. **[App crash debugging](ca://s?q=React_Native_app_crash_debugging)**  
   Your app crashes only on Android 12 devices. How do you systematically debug and isolate the issue?

2. **[Slow startup time](ca://s?q=React_Native_slow_startup_time)**  
   Users complain the app takes too long to launch. What steps would you take to profile and reduce startup time?

3. **[Network request failure](ca://s?q=React_Native_network_request_failure)**  
   API calls intermittently fail on poor connections. How would you implement retry logic and offline caching?

4. **[UI lag on scroll](ca://s?q=React_Native_UI_scroll_lag)**  
   A FlatList scroll stutters when rendering images. How do you optimize list rendering and image loading?

5. **[State management bug](ca://s?q=React_Native_state_management_bug)**  
   A Redux store update doesn’t reflect in the UI. How do you debug and fix state synchronization issues?

6. **[Push notification issue](ca://s?q=React_Native_push_notification_issue)**  
   Notifications arrive but don’t open the correct screen. How do you debug deep linking and navigation integration?

7. **[Memory leak detection](ca://s?q=React_Native_memory_leak_detection)**  
   The app’s memory usage keeps growing after navigation. How do you detect and fix memory leaks?

8. **[Gesture conflict](ca://s?q=React_Native_gesture_conflict)**  
   A swipe gesture conflicts with a scroll view. How do you resolve gesture handler conflicts?

9. **[Image upload failure](ca://s?q=React_Native_image_upload_failure)**  
   Large image uploads fail on mobile networks. How do you optimize uploads with compression and chunking?

10. **[OTA update rollback](ca://s?q=React_Native_OTA_update_rollback)**  
   An over-the-air update breaks the app for some users. How do you design a safe rollback strategy?

---

## 📊 Snapshot Table

| **[Problem](ca://s?q=React_Native_problem_solving)** | **Root Cause** | **Solution Approach** |
|----------------|-------------|----------------|
| App crash | OS-specific bug | Use logs, isolate version-specific APIs |
| Slow startup | Heavy bundle | Code splitting, lazy loading |
| Network failure | Poor connectivity | Retry logic, offline cache |
| UI lag | Excessive re-renders | Memoization, image caching |
| Memory leak | Unreleased listeners | Profiling, cleanup in `useEffect` |

---

## 🎯 Usage
This file can be used as:
- A **study guide** for React Native interviews  
- A **mock interview script** for practice  
- A **team exercise** to discuss debugging strategies
