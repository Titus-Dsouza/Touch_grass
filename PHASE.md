# TouchGrass — Development Phases

## Overview

This document outlines the development phases for TouchGrass, an AI-powered application designed to help users spend less time on screens and more time outside. Each phase builds upon the previous one, progressing from project setup to production-ready submission.

---

## Phase 1 — Project Setup

**Objective:** Establish the foundation for the project with proper configuration and repository structure.

### Tasks
- Set up GitHub repository
- Create frontend and backend directory structure
- Configure Django project and apps
- Set up Python virtual environment
- Configure environment variables (`.env` file)
- Add `.gitignore` for Python and Node.js dependencies

### Deliverables
- Repository initialized with proper structure
- Virtual environment ready for development
- All dependencies listed in `requirements.txt`
- Environment variables documented

### Exit Criteria
- Repo is accessible and organized
- Local development environment is ready

---

## Phase 2 — Frontend

**Objective:** Build a responsive, user-friendly interface with core components.

### Tasks
- Build landing page using HTML, CSS, and JavaScript
- Create responsive UI (mobile-first design)
- Implement chatbot interface
- Add outdoor mission cards
- Add "I'm Going Outside" button
- Ensure cross-browser compatibility

### Deliverables
- Landing page with hero section
- Chatbot UI component
- Mission card components
- Call-to-action button with proper styling
- Mobile-responsive layout

### Exit Criteria
- Frontend renders correctly on mobile and desktop
- All UI components are functional and styled
- No console errors or warnings

---

## Phase 3 — Authentication

**Objective:** Implement secure user authentication using Supabase.

### Tasks
- Create Supabase project
- Configure Supabase Authentication
- Implement signup flow
- Implement login flow
- Implement logout flow
- Handle user sessions and token management
- Add error handling for authentication

### Deliverables
- Supabase project configured
- Signup page with validation
- Login page with validation
- Session management on frontend
- User state persistence

### Exit Criteria
- Users can sign up with email/password
- Users can log in and maintain sessions
- Users can log out
- Protected routes work correctly

---

## Phase 4 — Django Backend

**Objective:** Build a robust REST API backend using Django and Django REST Framework.

### Tasks
- Set up Django REST Framework
- Create REST API endpoints
- Connect frontend with Django backend
- Implement authentication verification
- Create chatbot API endpoint
- Add request validation and error handling
- Configure CORS settings

### Deliverables
- Django REST API with endpoints for:
  - User authentication
  - User profiles
  - Chatbot interactions
  - Mission data
- API documentation
- Error handling and status codes

### Exit Criteria
- Frontend can communicate with backend
- All API endpoints are functional
- Authentication tokens are verified
- API responses follow consistent format

---

## Phase 5 — AI Chatbot

**Objective:** Build a chatbot service that interacts with users and encourages outdoor activities.

### Tasks
- Build chatbot service using Python
- Create system prompts and conversation flows
- Implement chatbot logic and response generation
- Connect chatbot with Django API endpoint
- Add response validation and error handling
- Implement conversation history tracking

### Deliverables
- Chatbot module with response generation
- Prompt templates for outdoor encouragement
- API endpoint for chatbot interactions
- Conversation context management
- Error handling for invalid inputs

### Exit Criteria
- Chatbot responds to user messages
- Responses are contextually appropriate
- Conversation history is maintained
- Integration with Django backend works

---

## Phase 6 — Open-Weight AI

**Objective:** Integrate an open-weight AI model for chatbot responses.

### Tasks
- Select an open-weight AI model (e.g., Llama 2, Mistral, OpenChat)
- Set up Ollama or alternative Python-compatible framework
- Configure model parameters and inference settings
- Connect the model to the chatbot service
- Test response quality and performance
- Optimize for latency and resource usage
- Document model selection rationale

### Deliverables
- Ollama/framework setup and configuration
- Integration with chatbot service
- Model performance benchmarks
- Response quality evaluation
- Documentation on model capabilities

### Exit Criteria
- Model responds to chatbot prompts
- Response quality meets requirements
- Response time is acceptable
- Model runs reliably without errors

---

## Phase 7 — Outdoor Mission Generation

**Objective:** Create a system to generate personalized outdoor missions.

### Tasks
- Design mission data model
- Generate personalized outdoor missions based on user preferences
- Display mission title, duration, and instructions
- Implement "I'm Going Outside" interaction tracking
- Create mission categories and difficulty levels
- Add mission completion rewards/tracking
- Encourage users to leave the website

### Deliverables
- Mission API endpoint
- Mission generation algorithm
- Mission card UI with call-to-action
- Mission tracking/completion system
- Success messaging

### Exit Criteria
- Missions are generated dynamically
- Users can view mission details
- "I'm Going Outside" action is tracked
- Users are encouraged to complete missions

---

## Phase 8 — Testing

**Objective:** Ensure all components work together reliably.

### Tasks
- Test authentication flow end-to-end
- Test chatbot functionality and responses
- Test API communication between frontend and backend
- Test AI model responses and performance
- Test mobile and desktop layouts
- Test error handling and edge cases
- Perform load testing
- Fix bugs and improve UI/UX

### Deliverables
- Test suite with unit and integration tests
- Bug fixes and improvements
- Performance optimization documentation
- Tested and stable build

### Exit Criteria
- All critical tests pass
- No known bugs in MVP features
- UI/UX is polished
- Application handles errors gracefully

---

## Phase 9 — Documentation

**Objective:** Create comprehensive documentation for users and contributors.

### Tasks
- Complete `README.md` with project overview and quick start
- Complete `ARCHITECTURE.md` with system design and component overview
- Complete `DESIGN.md` with UI/UX decisions and design system
- Complete `PRD.md` with product requirements and feature specifications
- Complete `PHASE.md` (this file) with development roadmap
- Add setup instructions (local and deployment)
- Add contribution guidelines
- Create API documentation

### Deliverables
- Professional README with badges and screenshots
- Architecture documentation with diagrams
- Design documentation with component library
- Product requirements document
- Contributing guide for open-source contributors

### Exit Criteria
- All documentation is complete and accurate
- Setup instructions work for new users
- Code comments explain complex logic
- Contribution process is clear

---

## Phase 10 — Hacktoberfest Submission

**Objective:** Prepare the project for Hacktoberfest and public release.

### Tasks
- Clean the repository (remove unused files, optimize assets)
- Verify and refine installation instructions
- Add screenshots and demo GIFs
- Create demo video or walkthrough
- Explain the use of open-source and open-weight AI models
- Add badges (license, open-source, open-weight AI)
- Test the complete project flow end-to-end
- Prepare submission documentation
- Set up GitHub discussions or community guidelines

### Deliverables
- Production-ready repository
- Visual demo materials (screenshots, GIFs, video)
- Clear value proposition and open-source messaging
- Complete onboarding documentation
- Hacktoberfest submission

### Exit Criteria
- Project is ready for public use
- Installation is simple and documented
- Benefits of open-weight AI are clear
- Community contribution guidelines are established

---

## MVP Goal

The MVP is considered **complete** when:

✅ Frontend is fully functional and responsive  
✅ Supabase authentication works reliably  
✅ Django backend API is operational  
✅ Python chatbot generates responses  
✅ Open-weight AI is successfully integrated  
✅ Outdoor missions are generated dynamically  
✅ Complete user flow works end-to-end  

### MVP User Flow
1. User visits the site and signs up/logs in
2. User chats with the AI chatbot about outdoor activities
3. Chatbot encourages outdoor participation
4. User receives a personalized outdoor mission
5. User clicks "I'm Going Outside" and leaves the platform

---

## Future Enhancements

After the MVP, consider these features:

- **User Preferences:** Store and personalize based on location, interests, fitness level
- **Mission History:** Track completed missions and achievements
- **Weather-Aware Activities:** Recommend activities based on current weather
- **Location-Aware Recommendations:** Suggest nearby parks, trails, and outdoor venues
- **Community Challenges:** Social features for group outdoor activities
- **Mobile App:** Native iOS/Android applications
- **Gamification:** Points, badges, leaderboards for outdoor activities
- **Integration:** Connect with fitness trackers and mapping services

---

## Timeline Estimate

- **Phases 1-2:** 1-2 weeks (setup & frontend)
- **Phases 3-4:** 1-2 weeks (auth & backend)
- **Phases 5-6:** 1-2 weeks (chatbot & AI)
- **Phase 7:** 1 week (missions)
- **Phase 8:** 1 week (testing & bug fixes)
- **Phase 9:** 1 week (documentation)
- **Phase 10:** 1 week (submission prep)

**Total Estimate:** 7-10 weeks for MVP completion

---

## Success Metrics

- MVP features are functional and bug-free
- User feedback is positive on UI/UX
- Open-weight AI model performs well (response quality, latency)
- Documentation is clear and helpful
- Community engagement (stars, forks, contributions)

---

## Mission Statement

> **Use AI to help people spend less time on screens and more time outside.**

This project succeeds when it measurably increases the time users spend outdoors while providing an enjoyable, engaging experience.
