### **🚀 Strato 3D Printing MVP Development Roadmap**
This roadmap outlines the step-by-step plan for building the **Strato 3D Printing MVP**, including backend APIs, frontend integration, and key features.  

---

## **📌 Phase 1: Authentication & Core API (✅ Completed)**
| **Task** | **Status** | **Details** |
|------------|------------|------------|
| **Set up Django + React repo & project structure** | ✅ Complete | Backend & frontend initialized |
| **User authentication (JWT login, register, logout)** | ✅ Complete | Users can sign up & sign in |
| **Role-based access (`IsUser`, `IsMaker`)** | ✅ Complete | Users & Makers have separate dashboards |
| **Test auth with frontend (`SignIn.tsx`, `Register.tsx`)** | ✅ Complete | Verified API integration |
| **Final debugging & API cleanup** | ✅ Complete | Ready for print job submission |

✅ **Outcome:** Authentication & user roles are fully working.

---

## **📌 Phase 2: Print Job Submission API & Frontend (✅ Completed)**
| **Task** | **Status** | **Details** |
|------------|------------|------------|
| **Create `PrintJob` model & API (`submit/`, `history/`, `status/`)** | ✅ Complete | Users submit jobs & view history |
| **Integrate with frontend (`PrintSubmit.tsx`, `PrintHistory.tsx`)** | ✅ Complete | Users submit jobs via UI |
| **Test job submission end-to-end** | ✅ Complete | Debugging & refine API |

✅ **Goal:** Users can submit print jobs & track status from the frontend.

---

## **📌 Phase 3: Lab & Printer Management (🔨 In Progress)**
| **Task** | **Status** | **Details** |
|------------|------------|------------|
| **Create `Lab` & `Printer` models + migrations** | 🔨 In Progress | Define structure for labs & printers |
| **Build API for makers to manage printers (`add/`, `update/`, `list/`)** | ⏳ Next | Makers add/update printers |
| **Integrate frontend (`LabSelect.tsx`, `PrinterList.tsx`)** | ⏳ Next | Makers manage printers via UI |
| **Update `PrintJob` submission to auto-assign printers** | ⏳ Next | Jobs get assigned to available printers |
| **Test auto-assignment of printers** | ⏳ Next | Debugging & finalizing logic |

✅ **Goal:** Makers manage printers, jobs get assigned automatically.

---

## **📌 Phase 4: Maker Job Management (⚙️ Two Weeks from Now)**
| **Task** | **Status** | **Details** |
|------------|------------|------------|
| **Build API for makers to view & update jobs (`manage/`, `update/`)** | ⏳ Next | Makers track & update job statuses |
| **Integrate frontend (`ReviewPrintRequest.tsx`)** | ⏳ Next | Makers manage print requests in UI |
| **Test updating job status (`pending → processing → completed`)** | ⏳ Next | Ensure job flow works smoothly |

✅ **Goal:** Makers fully control print job workflow.

---

## **📌 Phase 5: Notifications, Status Tracking & Final Testing (🔔 Final Week)**
| **Task** | **Status** | **Details** |
|------------|------------|------------|
| **Implement email/notification system (optional)** | ⏳ Next | Users get notified when jobs are ready |
| **Improve job status tracking & reassign failed prints** | ⏳ Next | Handle job failures & retry logic |
| **Full end-to-end testing with frontend** | ⏳ Next | Ensure everything works smoothly |

✅ **Goal:** A polished system that’s functional & user-friendly.

---

## **📌 Overall Timeline**
| **Phase** | **Target Completion** |
|------------|------------|
| ✅ **Phase 1: Authentication** | ✅ Completed |
| 🔥 **Phase 2: Print Job Submission** | ✅ Completed |
| ⚡ **Phase 3: Lab & Printer Management** | 🟡 **This Week**|
| ⚙️ **Phase 4: Maker Job Management** | 🟡 **Next Week** |
| 🔔 **Phase 5: Testing & Notifications** | 🟡 **Final Week** |

---


## **Bug Log**

| **Problem**                     | **Details**                                         | **Status**   |
|----------------------------------|-----------------------------------------------------|--------------|
| Post-registration redirect      | Tokens are only received on login; redirects to login after registration. | ⏳ Not Fixed  |


