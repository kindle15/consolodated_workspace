# Consolidated Workspace Manager

## 🎯 Initial Project Vision

**Goal**: Create a unified desktop workspace application that consolidates multiple development tools into a single, clutter-free interface—eliminating the need to juggle multiple windows and applications.

**Core Concept**: A Python-based desktop application that authenticates via USB API key, integrates GitHub login and AI chat functionality, provides a file tree explorer mimicking FTP structure, and includes a multi-tab code editor—all in one cohesive workspace that takes up 100% of the active screen while allowing the Windows taskbar to remain accessible.

---

## 📋 Project Overview

The Consolidated Workspace Manager is a desktop productivity tool designed to streamline development workflows by bringing together essential tools—GitHub integration, AI chat, file management, code editing, and terminal access—into a single unified interface. No more switching between multiple applications or managing cluttered desktops.

---

## ✨ Required Features

### 🔐 Authentication & Access
- **USB API Key Authentication**: Application checks for USB device containing GitHub API key file
- **Login Prompt**: If USB with API key not found, display prompt with specific filename required
- **GitHub Login Integration**: Once authenticated, automatic GitHub login using API key

### 💬 AI Chat Interface
- **Main Window Display**: GitHub Copilot Chat embedded in main window area
- **Current Web Version**: Redirect to current version of GitHub Copilot Chat (no toolbox view)
- **Compact Layout**: Chat interface uses no more than 1/3 screen width and 1/3 screen height
- **Resizable**: Automatic and manual width/height scaling

### 🎛️ Chat Control Panel
- **Radio Button Options**:
  - Download included files (archive backup files sent in chat)
  - Download code snippets as .txt files
  - Download/archive full chat conversation to .txt
- **Static Action Buttons**: Activate selected radio button choice

### 📂 File Tree Explorer (2nd Panel)
- **Repository Folder View**: Display repo structure mimicking FTP-style text tree
- **Child Folder Navigation**: Show nested folders and files
- **Two Action Buttons**:
  1. Create Folder
  2. Refresh View

### 📝 Multi-File Code Editor (3rd Panel - Right Side)
- **Tabbed Interface**: Tabs above editor area
- **Tab Navigation**: Left/right scrollable tabs for working with multiple files simultaneously
- **Editor Functionality**: Clone Notepad editor functions (search for small Python-based editor for easy adaptation)
- **Toolbar Options**: Include search functionality either in-window or above tabs

### 💻 Built-in Terminal
- **No Admin Rights**: Terminal operates without administrator privileges
- **Admin Warning**: Display message when focused if admin rights needed, referring user to system CMD
- **Reopen Functionality**: Button to close and reopen current terminal session
- **Save Warning**: Warn user to save unsaved work before terminal restart

### 🖥️ Window Management
- **100% Active Screen**: Workspace uses full screen real estate
- **Windows Taskbar Compatible**: Allow Windows auto-hide toolbar to appear over bottom of window
- **Not Always-on-Top**: Can be used alongside other system apps (Notepad, File Explorer, CMD, etc.)
- **Single Workspace Goal**: Eliminate need for multiple apps on taskbar/start menu

---

## 🔍 Research Questions Addressed

**Q: Is there already a project that fulfills most/all of these objectives?**
- Research conducted on existing solutions and component availability

**Q: Are there projects in parts that can be adapted and/or consolidated into this tool?**
- Evaluated libraries and frameworks for component reuse
- Identified potential consolidation opportunities

---

## 🛠️ Technology Stack

- **Language**: Python 3.9+
- **GUI Framework**: PyQt5
- **Window Management**: pywin32
- **Browser Integration**: Selenium
- **USB Detection**: psutil + WMI
- **Code Editor**: Python-based lightweight editor (to be selected)

---

## 📚 Project Documentation

This repository contains comprehensive planning documents:

1. **01_Technical_Specification.txt**
2. **02_Timeline_and_Gantt.txt**
3. **03_File_Structure.txt**
4. **04_Research_Libraries.txt**
5. **05_Educated_Conclusion.txt**

---

## 🚀 Project Status

**Status**: ✅ Planning & Research Phase Complete  
**Viability Score**: 85/100  
**Next Phase**: Development Implementation

---

## 👤 Author

**kindle15**  
GitHub: [@kindle15](https://github.com/kindle15)

---

**Last Updated**: 2026-02-15 06:24:58  
**Status**: Planning & Development Phase