<!-- Blogger-Friendly Top 1% Growth Tracker -->
<!-- Copy karून directly Blogger Page च्या HTML view मध्ये paste kara -->

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&amp;display=swap" rel="stylesheet"/>

<style>
/* Top 1% Growth Tracker - Complete Styles */
.tracker-wrapper * {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.tracker-wrapper {
  font-family: 'Poppins', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  background: #f9fafb;
  color: #1f2937;
  line-height: 1.6;
  border-radius: 12px;
  overflow: hidden;
  margin: 1rem 0;
}

body.dark-mode .tracker-wrapper {
  background: #111827;
  color: #f9fafb;
}

.tracker-header {
  background: linear-gradient(135deg, #10b981 0%, #06b6d4 100%);
  color: white;
  padding: 1.5rem 1rem;
  text-align: center;
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
}

.tracker-header h1 {
  font-size: 1.8rem;
  font-weight: 700;
  margin-bottom: 0.5rem;
}

.tracker-header p {
  font-size: 0.9rem;
  opacity: 0.95;
}

.nav-tabs {
  display: flex;
  overflow-x: auto;
  background: white;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  padding: 0.5rem;
  gap: 0.5rem;
  -webkit-overflow-scrolling: touch;
}

.nav-tab {
  padding: 0.75rem 1.5rem;
  border: none;
  background: transparent;
  color: #1f2937;
  cursor: pointer;
  border-radius: 8px;
  font-weight: 500;
  white-space: nowrap;
  transition: all 0.3s;
  font-size: 0.9rem;
  font-family: 'Poppins', sans-serif;
}

.nav-tab:hover {
  background: #f9fafb;
}

.nav-tab.active {
  background: linear-gradient(135deg, #10b981 0%, #06b6d4 100%);
  color: white;
}

.tracker-container {
  max-width: 1200px;
  margin: 2rem auto;
  padding: 0 1rem;
}

.card {
  background: white;
  border-radius: 12px;
  padding: 1.5rem;
  margin-bottom: 1.5rem;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s, box-shadow 0.3s;
}

body.dark-mode .card {
  background: #1f2937;
}

.card:hover {
  transform: translateY(-2px);
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
}

.card-title {
  font-size: 1.3rem;
  font-weight: 600;
  margin-bottom: 1rem;
  color: #10b981;
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.section {
  display: none;
}

.section.active {
  display: block;
  animation: fadeIn 0.5s;
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

.btn {
  padding: 0.75rem 1.5rem;
  border: none;
  border-radius: 8px;
  cursor: pointer;
  font-weight: 500;
  transition: all 0.3s;
  font-size: 0.95rem;
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  font-family: 'Poppins', sans-serif;
}

.btn-primary {
  background: linear-gradient(135deg, #10b981 0%, #06b6d4 100%);
  color: white;
}

.btn-primary:hover {
  transform: scale(1.05);
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
}

.btn-secondary {
  background: #f9fafb;
  color: #1f2937;
}

.btn-secondary:hover {
  background: #1f2937;
  color: white;
}

.tracker-input,
.tracker-textarea,
.tracker-select {
  width: 100%;
  padding: 0.75rem;
  border: 2px solid #f9fafb;
  border-radius: 8px;
  font-family: 'Poppins', sans-serif;
  font-size: 0.95rem;
  margin-bottom: 1rem;
  background: white;
  color: #1f2937;
  transition: border 0.3s;
}

body.dark-mode .tracker-input,
body.dark-mode .tracker-textarea,
body.dark-mode .tracker-select {
  background: #374151;
  color: #f9fafb;
  border-color: #4b5563;
}

.tracker-input:focus,
.tracker-textarea:focus,
.tracker-select:focus {
  outline: none;
  border-color: #10b981;
}

.tracker-textarea {
  min-height: 100px;
  resize: vertical;
}

.habit-item {
  display: flex;
  align-items: center;
  padding: 1rem;
  background: #f9fafb;
  border-radius: 8px;
  margin-bottom: 0.75rem;
  gap: 1rem;
}

body.dark-mode .habit-item {
  background: #374151;
}

.habit-checkbox {
  width: 24px;
  height: 24px;
  cursor: pointer;
}

.habit-label {
  flex: 1;
  font-weight: 500;
}

.habit-streak {
  background: linear-gradient(135deg, #10b981 0%, #06b6d4 100%);
  color: white;
  padding: 0.25rem 0.75rem;
  border-radius: 20px;
  font-size: 0.85rem;
  font-weight: 600;
}

.progress-bar {
  width: 100%;
  height: 30px;
  background: #f9fafb;
  border-radius: 15px;
  overflow: hidden;
  position: relative;
  margin-bottom: 1rem;
}

.progress-fill {
  height: 100%;
  background: linear-gradient(135deg, #10b981 0%, #06b6d4 100%);
  transition: width 0.5s ease;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-weight: 600;
  font-size: 0.85rem;
}

.mood-selector {
  display: flex;
  justify-content: space-around;
  gap: 1rem;
  margin: 1rem 0;
  flex-wrap: wrap;
}

.mood-option {
  font-size: 2.5rem;
  cursor: pointer;
  transition: transform 0.3s;
  opacity: 0.5;
}

.mood-option:hover,
.mood-option.selected {
  transform: scale(1.3);
  opacity: 1;
}

.stats-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1rem;
  margin-bottom: 1.5rem;
}

.stat-card {
  background: linear-gradient(135deg, #10b981 0%, #06b6d4 100%);
  color: white;
  padding: 1.5rem;
  border-radius: 12px;
  text-align: center;
}

.stat-value {
  font-size: 2.5rem;
  font-weight: 700;
  margin-bottom: 0.5rem;
}

.stat-label {
  font-size: 0.9rem;
  opacity: 0.9;
}

.quote-box {
  background: linear-gradient(135deg, #10b981 0%, #06b6d4 100%);
  color: white;
  padding: 2rem;
  border-radius: 12px;
  text-align: center;
  font-style: italic;
  margin-bottom: 1.5rem;
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
}

.quote-text {
  font-size: 1.1rem;
  line-height: 1.8;
  margin-bottom: 1rem;
}

.quote-author {
  font-size: 0.9rem;
  opacity: 0.9;
}

.tracker-footer {
  background: #1f2937;
  color: white;
  text-align: center;
  padding: 2rem 1rem;
  margin-top: 3rem;
}

.tracker-footer p {
  margin-bottom: 0.5rem;
}

.theme-toggle {
  position: fixed;
  bottom: 20px;
  right: 20px;
  background: linear-gradient(135deg, #10b981 0%, #06b6d4 100%);
  color: white;
  border: none;
  border-radius: 50%;
  width: 50px;
  height: 50px;
  font-size: 1.5rem;
  cursor: pointer;
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
  z-index: 1000;
  transition: transform 0.3s;
}

.theme-toggle:hover {
  transform: scale(1.1);
}

.goal-item,
.journal-entry {
  background: #f9fafb;
  padding: 1rem;
  border-radius: 8px;
  margin-bottom: 1rem;
}

body.dark-mode .goal-item,
body.dark-mode .journal-entry {
  background: #374151;
}

.goal-item {
  border-left: 4px solid #10b981;
}

.goal-item h4 {
  margin-bottom: 0.5rem;
  color: #10b981;
}

.journal-date {
  font-size: 0.85rem;
  color: #10b981;
  font-weight: 600;
  margin-bottom: 0.5rem;
}

.affirmation-card {
  background: linear-gradient(135deg, #10b981 0%, #06b6d4 100%);
  color: white;
  padding: 2rem;
  border-radius: 12px;
  text-align: center;
  font-size: 1.2rem;
  line-height: 1.8;
  margin-bottom: 1rem;
}

.life-wheel {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1rem;
  margin: 1rem 0;
}

.wheel-area {
  background: #f9fafb;
  padding: 1rem;
  border-radius: 8px;
}

body.dark-mode .wheel-area {
  background: #374151;
}

.wheel-area label {
  display: block;
  margin-bottom: 0.5rem;
  font-weight: 500;
}

.wheel-slider {
  width: 100%;
  margin-bottom: 0.5rem;
}

.vision-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
  gap: 1rem;
  margin: 1rem 0;
}

.vision-card {
  background: #f9fafb;
  padding: 1rem;
  border-radius: 8px;
  text-align: center;
  min-height: 150px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 500;
  position: relative;
}

body.dark-mode .vision-card {
  background: #374151;
}

/* Popup Styles */
.popup-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.7);
  z-index: 9999;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 1rem;
  animation: fadeIn 0.3s;
}

.popup-content {
  background: white;
  border-radius: 16px;
  max-width: 600px;
  width: 100%;
  max-height: 90vh;
  overflow-y: auto;
  box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
  animation: slideUp 0.3s;
}

body.dark-mode .popup-content {
  background: #1f2937;
}

@keyframes slideUp {
  from { transform: translateY(50px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}

.popup-header {
  background: linear-gradient(135deg, #10b981 0%, #06b6d4 100%);
  color: white;
  padding: 1.5rem;
  border-radius: 16px 16px 0 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.popup-header h2 {
  font-size: 1.5rem;
  font-weight: 700;
  margin: 0;
}

.popup-close {
  background: rgba(255, 255, 255, 0.2);
  border: none;
  color: white;
  font-size: 1.5rem;
  width: 36px;
  height: 36px;
  border-radius: 50%;
  cursor: pointer;
  transition: all 0.3s;
}

.popup-close:hover {
  background: rgba(255, 255, 255, 0.3);
  transform: rotate(90deg);
}

.popup-subtitle {
  font-size: 1.3rem;
  font-weight: 600;
  color: #1f2937;
  padding: 1.5rem 1.5rem 1rem 1.5rem;
  margin: 0;
}

body.dark-mode .popup-subtitle {
  color: #f9fafb;
}

.category-list {
  padding: 0 1.5rem 1.5rem 1.5rem;
}

.category-item {
  display: flex;
  align-items: center;
  padding: 1rem;
  border: 2px solid #e5e7eb;
  border-radius: 12px;
  margin-bottom: 0.75rem;
  cursor: pointer;
  transition: all 0.3s;
}

body.dark-mode .category-item {
  border-color: #374151;
}

.category-item:hover {
  border-color: #10b981;
  background: #f0fdf4;
  transform: translateX(5px);
}

body.dark-mode .category-item:hover {
  background: #374151;
}

.category-item input[type="radio"] {
  width: 24px;
  height: 24px;
  margin-right: 1rem;
  cursor: pointer;
  accent-color: #10b981;
}

.category-item label {
  font-size: 1.1rem;
  font-weight: 500;
  cursor: pointer;
  flex: 1;
  margin: 0;
}

.category-item.selected {
  border-color: #10b981;
  background: #f0fdf4;
}

body.dark-mode .category-item.selected {
  background: #065f46;
  border-color: #10b981;
}

@media (max-width: 768px) {
  .popup-content {
    max-height: 85vh;
  }
  
  .popup-header h2 {
    font-size: 1.2rem;
  }
  
  .category-item {
    padding: 0.75rem;
  }
  
  .category-item label {
    font-size: 1rem;
  }
}

@media (max-width: 768px) {
  .tracker-header h1 {
    font-size: 1.4rem;
  }
  .tracker-container {
    margin: 1rem auto;
    padding: 0 0.5rem;
  }
  .card {
    padding: 1rem;
  }
  .stats-grid {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="tracker-wrapper">
  <!-- Header -->
  <div class="tracker-header">
    <h1>🚀 Top 1% Growth Tracker</h1>
    <p>Every day you show up, you rise above the 99%. Keep going! 💪</p>
  </div>

  <!-- Navigation Tabs -->
  <div class="nav-tabs">
    <button class="nav-tab active" onclick="TrackerApp.showSection('dashboard')">🏠 Dashboard</button>
    <button class="nav-tab" onclick="TrackerApp.showSection('habits')">✅ Habits</button>
    <button class="nav-tab" onclick="TrackerApp.showSection('goals')">🎯 Goals</button>
    <button class="nav-tab" onclick="TrackerApp.showSection('journal')">📝 Journal</button>
    <button class="nav-tab" onclick="TrackerApp.showSection('gratitude')">🙏 Gratitude</button>
    <button class="nav-tab" onclick="TrackerApp.showSection('affirmations')">💫 Affirmations</button>
    <button class="nav-tab" onclick="TrackerApp.showSection('reflection')">🪞 Reflection</button>
    <button class="nav-tab" onclick="TrackerApp.showSection('lifewheel')">🎡 Life Wheel</button>
    <button class="nav-tab" onclick="TrackerApp.showSection('vision')">🌟 Vision</button>
    <button class="nav-tab" onclick="TrackerApp.showSection('settings')">⚙️ Settings</button>
  </div>

  <!-- Main Container -->
  <div class="tracker-container">
    <!-- DASHBOARD SECTION -->
    <div id="dashboard" class="section active">
      <!-- Stats Grid -->
      <div class="stats-grid">
        <div class="stat-card">
          <div class="stat-value" id="totalDays">0</div>
          <div class="stat-label">Days Active</div>
        </div>
        <div class="stat-card">
          <div class="stat-value" id="currentStreak">0</div>
          <div class="stat-label">Current Streak 🔥</div>
        </div>
        <div class="stat-card">
          <div class="stat-value" id="goalsCompleted">0</div>
          <div class="stat-label">Goals Achieved</div>
        </div>
      </div>

      <!-- Daily Quote -->
      <div class="quote-box">
        <div class="quote-text" id="dailyQuote">"Loading inspiration..."</div>
        <div class="quote-author" id="quoteAuthor"></div>
        <button class="btn btn-secondary" onclick="TrackerApp.loadNewQuote()" style="margin-top: 1rem;">🔄 New Quote</button>
      </div>

      <!-- Today's Affirmation -->
      <div class="card">
        <h3 class="card-title">💫 Today's Affirmation</h3>
        <div class="affirmation-card" id="dailyAffirmation">Loading...</div>
        <button class="btn btn-primary" onclick="TrackerApp.loadNewAffirmation()">🔄 New Affirmation</button>
      </div>

      <!-- Daily Mood Tracker -->
      <div class="card">
        <h3 class="card-title">😊 How are you feeling?</h3>
        <div class="mood-selector">
          <span class="mood-option" onclick="TrackerApp.setMood('😊', 'Happy')">😊</span>
          <span class="mood-option" onclick="TrackerApp.setMood('😌', 'Peaceful')">😌</span>
          <span class="mood-option" onclick="TrackerApp.setMood('💪', 'Motivated')">💪</span>
          <span class="mood-option" onclick="TrackerApp.setMood('🎯', 'Focused')">🎯</span>
          <span class="mood-option" onclick="TrackerApp.setMood('😰', 'Stressed')">😰</span>
          <span class="mood-option" onclick="TrackerApp.setMood('😔', 'Sad')">😔</span>
        </div>
        <p id="moodMessage" style="text-align: center; margin-top: 1rem; font-weight: 500;"></p>
      </div>

      <!-- Quick Actions -->
      <div class="card">
        <h3 class="card-title">⚡ Quick Actions</h3>
        <div style="display: flex; gap: 1rem; flex-wrap: wrap;">
          <button class="btn btn-primary" onclick="TrackerApp.showSection('habits')">✅ Log Habits</button>
          <button class="btn btn-primary" onclick="TrackerApp.showSection('journal')">📝 Write Journal</button>
          <button class="btn btn-primary" onclick="TrackerApp.showSection('gratitude')">🙏 Add Gratitude</button>
        </div>
      </div>
    </div>

    <!-- HABITS SECTION -->
    <div id="habits" class="section">
      <div class="card">
        <h3 class="card-title">✅ Daily Habits Tracker</h3>
        <div id="habitsList"></div>
        <button class="btn btn-primary" onclick="TrackerApp.addCustomHabit()">➕ Add Habit</button>
      </div>
      <div class="card">
        <h3 class="card-title">📊 Progress</h3>
        <div class="progress-bar">
          <div class="progress-fill" id="habitProgress" style="width: 0%">0%</div>
        </div>
        <p style="text-align: center; color: #10b981; font-weight: 600;">Keep going! 🔥</p>
      </div>
    </div>

    <!-- GOALS SECTION -->
    <div id="goals" class="section">
      <div class="card">
        <h3 class="card-title">🎯 My Goals</h3>
        <button class="btn btn-primary" onclick="TrackerApp.openCategoryPopup()" style="width: 100%; font-size: 1.1rem; padding: 1rem;">➕ Create New Goal</button>
      </div>
      <div class="card">
        <h3 class="card-title">📋 Current Goals</h3>
        <div id="goalsList"></div>
      </div>
    </div>

    <!-- Goal Category Popup -->
    <div id="categoryPopup" class="popup-overlay" style="display: none;">
      <div class="popup-content">
        <div class="popup-header">
          <h2>🎯 Goal Setting and Tracking</h2>
          <button class="popup-close" onclick="TrackerApp.closeCategoryPopup()">✕</button>
        </div>
        <h3 class="popup-subtitle">Create New Goal</h3>
        <div class="category-list">
          <div class="category-item" onclick="TrackerApp.selectCategory('Health', '💪')">
            <input type="radio" name="category" id="cat-health"/>
            <label for="cat-health">💪 Health</label>
          </div>
          <div class="category-item" onclick="TrackerApp.selectCategory('Wealth', '💰')">
            <input type="radio" name="category" id="cat-wealth"/>
            <label for="cat-wealth">💰 Wealth</label>
          </div>
          <div class="category-item" onclick="TrackerApp.selectCategory('Career', '💼')">
            <input type="radio" name="category" id="cat-career"/>
            <label for="cat-career">💼 Career</label>
          </div>
          <div class="category-item" onclick="TrackerApp.selectCategory('Finance', '💵')">
            <input type="radio" name="category" id="cat-finance"/>
            <label for="cat-finance">💵 Finance</label>
          </div>
          <div class="category-item" onclick="TrackerApp.selectCategory('Learning', '📚')">
            <input type="radio" name="category" id="cat-learning"/>
            <label for="cat-learning">📚 Learning</label>
          </div>
          <div class="category-item" onclick="TrackerApp.selectCategory('Relationships', '❤️')">
            <input type="radio" name="category" id="cat-relationships"/>
            <label for="cat-relationships">❤️ Relationships</label>
          </div>
          <div class="category-item" onclick="TrackerApp.selectCategory('Spirituality', '🧘')">
            <input type="radio" name="category" id="cat-spirituality"/>
            <label for="cat-spirituality">🧘 Spirituality</label>
          </div>
          <div class="category-item" onclick="TrackerApp.selectCategory('Mindset', '🧠')">
            <input type="radio" name="category" id="cat-mindset"/>
            <label for="cat-mindset">🧠 Mindset</label>
          </div>
          <div class="category-item" onclick="TrackerApp.selectCategory('Skills', '⚡')">
            <input type="radio" name="category" id="cat-skills"/>
            <label for="cat-skills">⚡ Skills</label>
          </div>
          <div class="category-item" onclick="TrackerApp.selectCategory('Adventure', '🌍')">
            <input type="radio" name="category" id="cat-adventure"/>
            <label for="cat-adventure">🌍 Adventure</label>
          </div>
          <div class="category-item" onclick="TrackerApp.selectCategory('Creativity', '🎨')">
            <input type="radio" name="category" id="cat-creativity"/>
            <label for="cat-creativity">🎨 Creativity</label>
          </div>
          <div class="category-item" onclick="TrackerApp.selectCategory('Family', '👨‍👩‍👧‍👦')">
            <input type="radio" name="category" id="cat-family"/>
            <label for="cat-family">👨‍👩‍👧‍👦 Family</label>
          </div>
          <div class="category-item" onclick="TrackerApp.selectCategory('Social Impact', '🤝')">
            <input type="radio" name="category" id="cat-social"/>
            <label for="cat-social">🤝 Social Impact</label>
          </div>
          <div class="category-item" onclick="TrackerApp.selectCategory('Personal Growth', '🌱')">
            <input type="radio" name="category" id="cat-growth"/>
            <label for="cat-growth">🌱 Personal Growth</label>
          </div>
          <div class="category-item" onclick="TrackerApp.selectCategory('Entertainment', '🎮')">
            <input type="radio" name="category" id="cat-entertainment"/>
            <label for="cat-entertainment">🎮 Entertainment</label>
          </div>
          <div class="category-item" onclick="TrackerApp.selectCategory('Other', '🎯')">
            <input type="radio" name="category" id="cat-other"/>
            <label for="cat-other">🎯 Other</label>
          </div>
        </div>
      </div>
    </div>

    <!-- Goal Details Popup -->
    <div id="goalDetailsPopup" class="popup-overlay" style="display: none;">
      <div class="popup-content">
        <div class="popup-header">
          <h2 id="selectedCategoryTitle">🎯 Create Goal</h2>
          <button class="popup-close" onclick="TrackerApp.closeGoalDetailsPopup()">✕</button>
        </div>
        <div style="padding: 1.5rem;">
          <input type="text" class="tracker-input" id="popupGoalTitle" placeholder="Goal title (e.g., Run 5km daily)"/>
          <textarea class="tracker-textarea" id="popupGoalDescription" placeholder="Describe your goal and why it matters to you..."></textarea>
          <select class="tracker-select" id="popupGoalPriority">
            <option value="high">🔴 High Priority</option>
            <option value="medium">🟡 Medium Priority</option>
            <option value="low">🟢 Low Priority</option>
          </select>
          <input type="date" class="tracker-input" id="popupGoalDeadline" placeholder="Target date (optional)"/>
          <button class="btn btn-primary" onclick="TrackerApp.saveGoalFromPopup()" style="width: 100%; margin-top: 1rem;">💾 Save Goal</button>
        </div>
      </div>
    </div>

    <!-- JOURNAL SECTION -->
    <div id="journal" class="section">
      <div class="card">
        <h3 class="card-title">📝 Daily Journal</h3>
        <p style="margin-bottom: 1rem; color: #10b981; font-weight: 500;">✨ What did you improve by 1% today?</p>
        <textarea class="tracker-textarea" id="journalEntry" placeholder="Write your thoughts..."></textarea>
        <button class="btn btn-primary" onclick="TrackerApp.saveJournalEntry()">💾 Save Entry</button>
      </div>
      <div class="card">
        <h3 class="card-title">📖 Previous Entries</h3>
        <div id="journalList"></div>
      </div>
    </div>

    <!-- GRATITUDE SECTION -->
    <div id="gratitude" class="section">
      <div class="card">
        <h3 class="card-title">🙏 Daily Gratitude</h3>
        <p style="margin-bottom: 1rem;">List 3 things you're grateful for:</p>
        <input type="text" class="tracker-input" id="gratitude1" placeholder="1. I'm grateful for..."/>
        <input type="text" class="tracker-input" id="gratitude2" placeholder="2. I'm grateful for..."/>
        <input type="text" class="tracker-input" id="gratitude3" placeholder="3. I'm grateful for..."/>
        <button class="btn btn-primary" onclick="TrackerApp.saveGratitude()">💚 Save Gratitude</button>
      </div>
      <div class="card">
        <h3 class="card-title">💖 Gratitude History</h3>
        <div id="gratitudeList"></div>
      </div>
    </div>

    <!-- AFFIRMATIONS SECTION -->
    <div id="affirmations" class="section">
      <div class="card">
        <h3 class="card-title">💫 My Personal Affirmations</h3>
        <textarea class="tracker-textarea" id="customAffirmation" placeholder="Write your affirmation..."></textarea>
        <button class="btn btn-primary" onclick="TrackerApp.addCustomAffirmation()">➕ Add Affirmation</button>
      </div>
      <div class="card">
        <h3 class="card-title">✨ Your Affirmations</h3>
        <div id="affirmationsList"></div>
      </div>
      <div class="card">
        <h3 class="card-title">🎯 1% Mindset Library</h3>
        <button class="btn btn-primary" onclick="TrackerApp.showRandomAffirmation()">🎲 Random Affirmation</button>
        <div id="randomAffirmationDisplay" style="margin-top: 1rem;"></div>
      </div>
    </div>

    <!-- REFLECTION SECTION -->
    <div id="reflection" class="section">
      <div class="card">
        <h3 class="card-title">🪞 Weekly Reflection</h3>
        <label style="display: block; margin-bottom: 0.5rem; font-weight: 500;">What went well?</label>
        <textarea class="tracker-textarea" id="reflectionWins" placeholder="Celebrate your wins..."></textarea>
        <label style="display: block; margin-bottom: 0.5rem; font-weight: 500;">What needs improvement?</label>
        <textarea class="tracker-textarea" id="reflectionImprovement" placeholder="Areas to work on..."></textarea>
        <label style="display: block; margin-bottom: 0.5rem; font-weight: 500;">Next week's focus?</label>
        <textarea class="tracker-textarea" id="reflectionFocus" placeholder="Your focus..."></textarea>
        <button class="btn btn-primary" onclick="TrackerApp.saveReflection()">💾 Save Reflection</button>
      </div>
      <div class="card">
        <h3 class="card-title">📊 Past Reflections</h3>
        <div id="reflectionList"></div>
      </div>
    </div>

    <!-- LIFE WHEEL SECTION -->
    <div id="lifewheel" class="section">
      <div class="card">
        <h3 class="card-title">🎡 Life Balance Wheel</h3>
        <p style="margin-bottom: 1rem;">Rate each area (1-10):</p>
        <div class="life-wheel">
          <div class="wheel-area">
            <label>🧠 Mindset: <span id="mindsetValue">5</span></label>
            <input type="range" class="wheel-slider" min="1" max="10" value="5" id="mindsetSlider" oninput="TrackerApp.updateSlider('mindset', this.value)"/>
          </div>
          <div class="wheel-area">
            <label>💪 Health: <span id="healthValue">5</span></label>
            <input type="range" class="wheel-slider" min="1" max="10" value="5" id="healthSlider" oninput="TrackerApp.updateSlider('health', this.value)"/>
          </div>
          <div class="wheel-area">
            <label>💖 Relationships: <span id="relationshipsValue">5</span></label>
            <input type="range" class="wheel-slider" min="1" max="10" value="5" id="relationshipsSlider" oninput="TrackerApp.updateSlider('relationships', this.value)"/>
          </div>
          <div class="wheel-area">
            <label>💼 Career: <span id="careerValue">5</span></label>
            <input type="range" class="wheel-slider" min="1" max="10" value="5" id="careerSlider" oninput="TrackerApp.updateSlider('career', this.value)"/>
          </div>
          <div class="wheel-area">
            <label>💰 Finance: <span id="financeValue">5</span></label>
            <input type="range" class="wheel-slider" min="1" max="10" value="5" id="financeSlider" oninput="TrackerApp.updateSlider('finance', this.value)"/>
          </div>
          <div class="wheel-area">
            <label>🙏 Spirituality: <span id="spiritualityValue">5</span></label>
            <input type="range" class="wheel-slider" min="1" max="10" value="5" id="spiritualitySlider" oninput="TrackerApp.updateSlider('spirituality', this.value)"/>
          </div>
          <div class="wheel-area">
            <label>😊 Emotions: <span id="emotionsValue">5</span></label>
            <input type="range" class="wheel-slider" min="1" max="10" value="5" id="emotionsSlider" oninput="TrackerApp.updateSlider('emotions', this.value)"/>
          </div>
          <div class="wheel-area">
            <label>🌟 Lifestyle: <span id="lifestyleValue">5</span></label>
            <input type="range" class="wheel-slider" min="1" max="10" value="5" id="lifestyleSlider" oninput="TrackerApp.updateSlider('lifestyle', this.value)"/>
          </div>
        </div>
        <button class="btn btn-primary" onclick="TrackerApp.saveLifeWheel()">💾 Save Life Balance</button>
      </div>
      <div class="card">
        <h3 class="card-title">📈 Overall Balance Score</h3>
        <div class="stat-card" style="margin: 0;">
          <div class="stat-value" id="balanceScore">40</div>
          <div class="stat-label">out of 80</div>
        </div>
      </div>
    </div>

    <!-- VISION BOARD SECTION -->
    <div id="vision" class="section">
      <div class="card">
        <h3 class="card-title">🌟 Vision Board</h3>
        <p style="margin-bottom: 1rem;">Add your goals and dreams:</p>
        <input type="text" class="tracker-input" id="visionItem" placeholder="Enter a goal or dream..."/>
        <button class="btn btn-primary" onclick="TrackerApp.addVisionItem()">➕ Add to Vision Board</button>
      </div>
      <div class="card">
        <h3 class="card-title">✨ Your Vision</h3>
        <div class="vision-grid" id="visionGrid"></div>
      </div>
    </div>

    <!-- SETTINGS SECTION -->
    <div id="settings" class="section">
      <div class="card">
        <h3 class="card-title">⚙️ Settings</h3>
        <h4 style="margin: 1rem 0;">🌙 Theme</h4>
        <button class="btn btn-primary" onclick="TrackerApp.toggleTheme()">🌓 Toggle Dark/Light Mode</button>
        <h4 style="margin: 1.5rem 0 1rem 0;">📥 Data Management</h4>
        <button class="btn btn-primary" onclick="TrackerApp.exportData()" style="margin-right: 0.5rem; margin-bottom: 0.5rem;">📥 Export Data</button>
        <button class="btn btn-secondary" onclick="TrackerApp.importData()" style="margin-right: 0.5rem; margin-bottom: 0.5rem;">📤 Import Data</button>
        <button class="btn btn-secondary" onclick="TrackerApp.resetAllData()" style="background: #ef4444; color: white; margin-bottom: 0.5rem;">🗑️ Reset All Data</button>
        <h4 style="margin: 1.5rem 0 1rem 0;">ℹ️ About</h4>
        <p>Version 1.0 - Built with 💚 by Grow With Rupesh</p>
        <p style="margin-top: 0.5rem;">All data stored locally for privacy.</p>
      </div>
    </div>
  </div>

  <!-- Footer -->
  <div class="tracker-footer">
    <p>💪 "Every day you show up, you rise above the 99%"</p>
    <p style="font-size: 0.9rem; opacity: 0.9; margin-top: 0.5rem;">Made with ❤️ by <strong>Grow With Rupesh</strong></p>
    <p style="font-size: 0.85rem; opacity: 0.8; margin-top: 0.5rem;">🚀 Your 1% daily improvement compounds into extraordinary results</p>
  </div>

  <!-- Theme Toggle Button -->
  <button class="theme-toggle" onclick="TrackerApp.toggleTheme()">🌓</button>
</div>

<script>
//<![CDATA[
// Top 1% Growth Tracker - Complete JavaScript
(function() {
  'use strict';

  // ===== DATA ARRAYS =====
  const AFFIRMATIONS = [
    "I am becoming 1% better every single day.",
    "Consistency is my superpower.",
    "I am focused, disciplined, and unstoppable.",
    "My actions today create my success tomorrow.",
    "I choose growth over comfort.",
    "I am the architect of my life.",
    "Every challenge strengthens my mindset.",
    "I control my thoughts, emotions, and habits.",
    "I show up even when I don't feel like it.",
    "I am worthy of greatness.",
    "I trust the process of self-improvement.",
    "I am disciplined in my thoughts and actions.",
    "I learn something new every day.",
    "I am grateful for every opportunity to grow.",
    "I am not afraid to fail; I am afraid not to try.",
    "My focus creates my future.",
    "I am in control of my time and energy.",
    "I am proud of how far I've come.",
    "My growth never stops.",
    "I believe in long-term success over short-term comfort.",
    "I am a learner, a doer, and a leader.",
    "I don't compare; I improve.",
    "I am patient and persistent.",
    "I attract success through my habits.",
    "I honor my commitments to myself.",
    "I am becoming my highest version.",
    "I value progress more than perfection.",
    "I take full responsibility for my life.",
    "My daily habits define my destiny.",
    "I am unstoppable because I never give up.",
    "I work in silence; my success will speak.",
    "I am committed to mastery.",
    "I build momentum through small wins.",
    "I am resilient and adaptable.",
    "I am focused on my mission.",
    "I invest my time wisely.",
    "I respect my routine.",
    "I move with intention and clarity.",
    "I am calm, confident, and courageous.",
    "My mind is my greatest weapon.",
    "I see discomfort as growth.",
    "I am building a legacy of excellence.",
    "I am proud of my discipline.",
    "I attract abundance through gratitude.",
    "I am constantly learning and evolving.",
    "I choose peace over chaos.",
    "I act now; I don't wait for the perfect time.",
    "I am my only competition.",
    "My consistency compounds into success.",
    "I am designed for greatness."
  ];

  const QUOTES = [
    { text: "Discipline is the bridge between goals and accomplishment.", author: "Jim Rohn" },
    { text: "You'll never change your life until you change something you do daily.", author: "John C. Maxwell" },
    { text: "The secret of your future is hidden in your daily routine.", author: "Mike Murdock" },
    { text: "Success is nothing more than a few simple disciplines practiced every day.", author: "Jim Rohn" },
    { text: "Small daily improvements lead to stunning results.", author: "Robin Sharma" },
    { text: "The difference between ordinary and extraordinary is consistency.", author: "Unknown" },
    { text: "Discipline equals freedom.", author: "Jocko Willink" },
    { text: "Do something today that your future self will thank you for.", author: "Unknown" },
    { text: "Your habits define your future.", author: "Unknown" },
    { text: "Dream big. Start small. Act now.", author: "Robin Sharma" },
    { text: "You can't cheat the grind.", author: "Eric Thomas" },
    { text: "Success is not final, failure is not fatal; it's the courage to continue that counts.", author: "Winston Churchill" },
    { text: "Be addicted to bettering yourself.", author: "Unknown" },
    { text: "The future depends on what you do today.", author: "Mahatma Gandhi" },
    { text: "You become what you repeatedly do.", author: "Aristotle" }
  ];

  const DEFAULT_HABITS = [
    { name: "🧘 Morning Meditation", completed: false, streak: 0 },
    { name: "📚 Read for 30 minutes", completed: false, streak: 0 },
    { name: "💪 Exercise", completed: false, streak: 0 },
    { name: "📝 Journal", completed: false, streak: 0 },
    { name: "💧 Drink 8 glasses of water", completed: false, streak: 0 },
    { name: "🎯 Work on main goal", completed: false, streak: 0 }
  ];

  // ===== STATE MANAGEMENT =====
  let appData = {
    habits: [],
    goals: [],
    journal: [],
    gratitude: [],
    customAffirmations: [],
    reflections: [],
    lifeWheel: {},
    visionBoard: [],
    stats: {
      totalDays: 0,
      currentStreak: 0,
      goalsCompleted: 0,
      lastVisit: null
    },
    todaysMood: null,
    theme: 'light',
    selectedCategory: null,
    selectedCategoryIcon: null
  };

  // ===== LOCAL STORAGE =====
  function saveData() {
    try {
      localStorage.setItem('top1PercentData', JSON.stringify(appData));
    } catch (e) {
      console.error('Save error:', e);
    }
  }

  function loadData() {
    try {
      const saved = localStorage.getItem('top1PercentData');
      if (saved) {
        appData = JSON.parse(saved);
      } else {
        appData.habits = JSON.parse(JSON.stringify(DEFAULT_HABITS));
      }
    } catch (e) {
      console.error('Load error:', e);
      appData.habits = JSON.parse(JSON.stringify(DEFAULT_HABITS));
    }
  }

  // ===== NAVIGATION =====
  function showSection(sectionId) {
    const sections = document.querySelectorAll('.section');
    const tabs = document.querySelectorAll('.nav-tab');
    
    sections.forEach(function(s) { s.classList.remove('active'); });
    tabs.forEach(function(t) { t.classList.remove('active'); });
    
    const targetSection = document.getElementById(sectionId);
    if (targetSection) targetSection.classList.add('active');
    
    if (window.event && window.event.target) {
      window.event.target.classList.add('active');
    }
  }

  // ===== QUOTES & AFFIRMATIONS =====
  function loadDailyQuote() {
    const quote = QUOTES[Math.floor(Math.random() * QUOTES.length)];
    const el = document.getElementById('dailyQuote');
    const auth = document.getElementById('quoteAuthor');
    if (el) el.textContent = '"' + quote.text + '"';
    if (auth) auth.textContent = '— ' + quote.author;
  }

  function loadNewQuote() {
    loadDailyQuote();
  }

  function loadDailyAffirmation() {
    const aff = AFFIRMATIONS[Math.floor(Math.random() * AFFIRMATIONS.length)];
    const el = document.getElementById('dailyAffirmation');
    if (el) el.textContent = aff;
  }

  function loadNewAffirmation() {
    loadDailyAffirmation();
  }

  function showRandomAffirmation() {
    const aff = AFFIRMATIONS[Math.floor(Math.random() * AFFIRMATIONS.length)];
    const el = document.getElementById('randomAffirmationDisplay');
    if (el) {
      el.innerHTML = '<div class="affirmation-card">' + aff + '</div>';
    }
  }

  // ===== MOOD TRACKING =====
  function setMood(emoji, mood) {
    appData.todaysMood = { emoji: emoji, mood: mood, date: new Date().toISOString() };
    
    const moods = document.querySelectorAll('.mood-option');
    moods.forEach(function(m) { m.classList.remove('selected'); });
    
    if (window.event && window.event.target) {
      window.event.target.classList.add('selected');
    }
    
    const messages = {
      'Happy': 'Wonderful! Keep spreading that positive energy! 😊',
      'Peaceful': 'Beautiful! Peace is the foundation of growth. 😌',
      'Motivated': 'Yes! Channel that energy into your goals! 💪',
      'Focused': 'Perfect! Stay in the zone and make magic happen! 🎯',
      'Stressed': 'Take a deep breath. You\'ve got this. One step at a time. 🌟',
      'Sad': 'It\'s okay to feel this way. Tomorrow is a new opportunity. 💚'
    };
    
    const el = document.getElementById('moodMessage');
    if (el) el.textContent = messages[mood] || 'Mood saved! 🌟';
    saveData();
  }

  // ===== HABITS =====
  function renderHabits() {
    const container = document.getElementById('habitsList');
    if (!container) return;
    container.innerHTML = '';
    
    appData.habits.forEach(function(habit, index) {
      const div = document.createElement('div');
      div.className = 'habit-item';
      div.innerHTML = '<input type="checkbox" class="habit-checkbox" ' + (habit.completed ? 'checked' : '') + ' onchange="TrackerApp.toggleHabit(' + index + ')"><span class="habit-label">' + habit.name + '</span><span class="habit-streak">' + habit.streak + ' 🔥</span>';
      container.appendChild(div);
    });
    
    updateHabitProgress();
  }

  function toggleHabit(index) {
    appData.habits[index].completed = !appData.habits[index].completed;
    saveData();
    renderHabits();
  }

  function updateHabitProgress() {
    const completed = appData.habits.filter(function(h) { return h.completed; }).length;
    const total = appData.habits.length;
    const percentage = total > 0 ? Math.round((completed / total) * 100) : 0;
    
    const bar = document.getElementById('habitProgress');
    if (bar) {
      bar.style.width = percentage + '%';
      bar.textContent = percentage + '%';
    }
  }

  function addCustomHabit() {
    const name = prompt('Enter habit name (e.g., 📖 Read 30 pages):');
    if (name && name.trim()) {
      appData.habits.push({ name: name.trim(), completed: false, streak: 0 });
      saveData();
      renderHabits();
    }
  }

  // ===== GOALS =====
  function renderGoals() {
    const container = document.getElementById('goalsList');
    if (!container) return;
    
    if (appData.goals.length === 0) {
      container.innerHTML = '<p style="text-align: center; color: #10b981;">No goals yet. Click "Create New Goal" to start! 🎯</p>';
      return;
    }
    
    container.innerHTML = '';
    appData.goals.forEach(function(goal, index) {
      const priorityColors = { high: '🔴', medium: '🟡', low: '🟢' };
      const div = document.createElement('div');
      div.className = 'goal-item';
      var categoryBadge = goal.category ? '<span class="badge">' + goal.categoryIcon + ' ' + goal.category + '</span>' : '';
      var deadlineText = goal.deadline ? '<p style="font-size: 0.85rem; color: #6b7280; margin-top: 0.5rem;">📅 Target: ' + new Date(goal.deadline).toLocaleDateString() + '</p>' : '';
      div.innerHTML = '<div style="display: flex; justify-content: space-between; align-items: start; margin-bottom: 0.5rem;"><h4 style="margin: 0;">' + priorityColors[goal.priority] + ' ' + goal.title + '</h4>' + categoryBadge + '</div><p>' + goal.description + '</p>' + deadlineText + '<div style="margin-top: 0.5rem;"><button class="btn btn-secondary" onclick="TrackerApp.completeGoal(' + index + ')" style="padding: 0.5rem 1rem; font-size: 0.85rem;">✅ Complete</button> <button class="btn btn-secondary" onclick="TrackerApp.deleteGoal(' + index + ')" style="padding: 0.5rem 1rem; font-size: 0.85rem; background: #ef4444; color: white;">🗑️ Delete</button></div>';
      container.appendChild(div);
    });
  }

  function openCategoryPopup() {
    const popup = document.getElementById('categoryPopup');
    if (popup) {
      popup.style.display = 'flex';
      document.body.style.overflow = 'hidden';
    }
  }

  function closeCategoryPopup() {
    const popup = document.getElementById('categoryPopup');
    if (popup) {
      popup.style.display = 'none';
      document.body.style.overflow = 'auto';
    }
  }

  function selectCategory(category, icon) {
    appData.selectedCategory = category;
    appData.selectedCategoryIcon = icon;
    
    // Highlight selected category
    var items = document.querySelectorAll('.category-item');
    items.forEach(function(item) {
      item.classList.remove('selected');
    });
    if (window.event && window.event.currentTarget) {
      window.event.currentTarget.classList.add('selected');
    }
    
    // Check the radio button
    var radios = document.querySelectorAll('.category-item input[type="radio"]');
    radios.forEach(function(radio) {
      radio.checked = false;
    });
    if (window.event && window.event.currentTarget) {
      var radio = window.event.currentTarget.querySelector('input[type="radio"]');
      if (radio) radio.checked = true;
    }
    
    // Open goal details popup after short delay
    setTimeout(function() {
      closeCategoryPopup();
      openGoalDetailsPopup();
    }, 300);
  }

  function openGoalDetailsPopup() {
    const popup = document.getElementById('goalDetailsPopup');
    const title = document.getElementById('selectedCategoryTitle');
    
    if (popup && title) {
      title.textContent = appData.selectedCategoryIcon + ' ' + appData.selectedCategory + ' Goal';
      popup.style.display = 'flex';
      document.body.style.overflow = 'hidden';
    }
  }

  function closeGoalDetailsPopup() {
    const popup = document.getElementById('goalDetailsPopup');
    if (popup) {
      popup.style.display = 'none';
      document.body.style.overflow = 'auto';
    }
    
    // Clear form
    var titleInput = document.getElementById('popupGoalTitle');
    var descInput = document.getElementById('popupGoalDescription');
    var deadlineInput = document.getElementById('popupGoalDeadline');
    if (titleInput) titleInput.value = '';
    if (descInput) descInput.value = '';
    if (deadlineInput) deadlineInput.value = '';
    
    appData.selectedCategory = null;
    appData.selectedCategoryIcon = null;
  }

  function saveGoalFromPopup() {
    const title = document.getElementById('popupGoalTitle');
    const description = document.getElementById('popupGoalDescription');
    const priority = document.getElementById('popupGoalPriority');
    const deadline = document.getElementById('popupGoalDeadline');
    
    if (!title || !title.value.trim()) {
      alert('Please enter a goal title!');
      return;
    }
    
    appData.goals.push({
      title: title.value.trim(),
      description: description ? description.value.trim() : '',
      priority: priority ? priority.value : 'medium',
      category: appData.selectedCategory,
      categoryIcon: appData.selectedCategoryIcon,
      deadline: deadline ? deadline.value : null,
      date: new Date().toISOString()
    });
    
    saveData();
    renderGoals();
    closeGoalDetailsPopup();
    alert('🎉 Goal created successfully! Keep pushing forward!');
  }

  function addGoal() {
    const title = document.getElementById('goalTitle');
    const description = document.getElementById('goalDescription');
    const priority = document.getElementById('goalPriority');
    
    if (!title || !title.value.trim()) {
      alert('Please enter a goal title!');
      return;
    }
    
    appData.goals.push({
      title: title.value.trim(),
      description: description ? description.value.trim() : '',
      priority: priority ? priority.value : 'medium',
      date: new Date().toISOString()
    });
    
    title.value = '';
    if (description) description.value = '';
    saveData();
    renderGoals();
  }

  function completeGoal(index) {
    if (confirm('Congratulations! 🎉 Mark this goal as completed?')) {
      appData.stats.goalsCompleted++;
      appData.goals.splice(index, 1);
      saveData();
      renderGoals();
      updateStats();
    }
  }

  function deleteGoal(index) {
    if (confirm('Are you sure you want to delete this goal?')) {
      appData.goals.splice(index, 1);
      saveData();
      renderGoals();
    }
  }

  // ===== JOURNAL =====
  function renderJournal() {
    const container = document.getElementById('journalList');
    if (!container) return;
    
    if (appData.journal.length === 0) {
      container.innerHTML = '<p style="text-align: center; color: #10b981;">No entries yet. Start writing! ✍️</p>';
      return;
    }
    
    container.innerHTML = '';
    var reversed = appData.journal.slice().reverse();
    reversed.forEach(function(entry) {
      const div = document.createElement('div');
      div.className = 'journal-entry';
      const date = new Date(entry.date);
      div.innerHTML = '<div class="journal-date">' + date.toLocaleDateString() + '</div><p>' + entry.content + '</p>';
      container.appendChild(div);
    });
  }

  function saveJournalEntry() {
    const input = document.getElementById('journalEntry');
    if (!input || !input.value.trim()) {
      alert('Please write something first!');
      return;
    }
    
    appData.journal.push({
      content: input.value.trim(),
      date: new Date().toISOString()
    });
    
    input.value = '';
    saveData();
    renderJournal();
    alert('Journal entry saved! 📝');
  }

  // ===== GRATITUDE =====
  function renderGratitude() {
    const container = document.getElementById('gratitudeList');
    if (!container) return;
    
    if (appData.gratitude.length === 0) {
      container.innerHTML = '<p style="text-align: center; color: #10b981;">No gratitude entries yet. Start today! 🙏</p>';
      return;
    }
    
    container.innerHTML = '';
    var reversed = appData.gratitude.slice().reverse();
    reversed.forEach(function(entry) {
      const div = document.createElement('div');
      div.className = 'journal-entry';
      const date = new Date(entry.date);
      div.innerHTML = '<div class="journal-date">' + date.toLocaleDateString() + '</div><p>1. ' + entry.items[0] + '</p><p>2. ' + entry.items[1] + '</p><p>3. ' + entry.items[2] + '</p>';
      container.appendChild(div);
    });
  }

  function saveGratitude() {
    const g1 = document.getElementById('gratitude1');
    const g2 = document.getElementById('gratitude2');
    const g3 = document.getElementById('gratitude3');
    
    if (!g1 || !g2 || !g3 || !g1.value.trim() || !g2.value.trim() || !g3.value.trim()) {
      alert('Please fill in all 3 gratitude items!');
      return;
    }
    
    appData.gratitude.push({
      items: [g1.value.trim(), g2.value.trim(), g3.value.trim()],
      date: new Date().toISOString()
    });
    
    g1.value = '';
    g2.value = '';
    g3.value = '';
    saveData();
    renderGratitude();
    alert('Gratitude saved! 💚 Keep the positive energy flowing!');
  }

  // ===== AFFIRMATIONS =====
  function renderAffirmations() {
    const container = document.getElementById('affirmationsList');
    if (!container) return;
    
    if (appData.customAffirmations.length === 0) {
      container.innerHTML = '<p style="text-align: center; color: #10b981;">No custom affirmations yet. Create your own! ✨</p>';
      return;
    }
    
    container.innerHTML = '';
    appData.customAffirmations.forEach(function(affirmation, index) {
      const div = document.createElement('div');
      div.className = 'affirmation-card';
      div.innerHTML = affirmation + '<button class="btn btn-secondary" onclick="TrackerApp.deleteAffirmation(' + index + ')" style="margin-top: 1rem; padding: 0.5rem 1rem; font-size: 0.85rem;">🗑️ Delete</button>';
      container.appendChild(div);
    });
  }

  function addCustomAffirmation() {
    const input = document.getElementById('customAffirmation');
    if (!input || !input.value.trim()) {
      alert('Please write an affirmation first!');
      return;
    }
    
    appData.customAffirmations.push(input.value.trim());
    input.value = '';
    saveData();
    renderAffirmations();
  }

  function deleteAffirmation(index) {
    appData.customAffirmations.splice(index, 1);
    saveData();
    renderAffirmations();
  }

  // ===== REFLECTIONS =====
  function renderReflections() {
    const container = document.getElementById('reflectionList');
    if (!container) return;
    
    if (appData.reflections.length === 0) {
      container.innerHTML = '<p style="text-align: center; color: #10b981;">No reflections yet. Take time to reflect weekly! 🪞</p>';
      return;
    }
    
    container.innerHTML = '';
    var reversed = appData.reflections.slice().reverse();
    reversed.forEach(function(reflection) {
      const div = document.createElement('div');
      div.className = 'journal-entry';
      const date = new Date(reflection.date);
      div.innerHTML = '<div class="journal-date">' + date.toLocaleDateString() + '</div><p><strong>✅ Wins:</strong> ' + reflection.wins + '</p><p><strong>📈 Improvement:</strong> ' + reflection.improvement + '</p><p><strong>🎯 Next Focus:</strong> ' + reflection.focus + '</p>';
      container.appendChild(div);
    });
  }

  function saveReflection() {
    const wins = document.getElementById('reflectionWins');
    const improvement = document.getElementById('reflectionImprovement');
    const focus = document.getElementById('reflectionFocus');
    
    if (!wins || !improvement || !focus || !wins.value.trim() || !improvement.value.trim() || !focus.value.trim()) {
      alert('Please fill in all reflection fields!');
      return;
    }
    
    appData.reflections.push({
      wins: wins.value.trim(),
      improvement: improvement.value.trim(),
      focus: focus.value.trim(),
      date: new Date().toISOString()
    });
    
    wins.value = '';
    improvement.value = '';
    focus.value = '';
    saveData();
    renderReflections();
    alert('Reflection saved! 🪞 Keep growing!');
  }

  // ===== LIFE WHEEL =====
  function updateSlider(area, value) {
    const el = document.getElementById(area + 'Value');
    if (el) el.textContent = value;
    appData.lifeWheel[area] = parseInt(value);
    updateBalanceScore();
  }

  function updateBalanceScore() {
    var total = 0;
    for (var key in appData.lifeWheel) {
      total += appData.lifeWheel[key];
    }
    const el = document.getElementById('balanceScore');
    if (el) el.textContent = total;
  }

  function saveLifeWheel() {
    saveData();
    alert('Life balance saved! 🎡 Keep working on all areas!');
  }

  // ===== VISION BOARD =====
  function renderVisionBoard() {
    const container = document.getElementById('visionGrid');
    if (!container) return;
    
    if (appData.visionBoard.length === 0) {
      container.innerHTML = '<p style="text-align: center; color: #10b981; grid-column: 1/-1;">No vision items yet. Start visualizing! 🌟</p>';
      return;
    }
    
    container.innerHTML = '';
    appData.visionBoard.forEach(function(item, index) {
      const div = document.createElement('div');
      div.className = 'vision-card';
      div.innerHTML = item + '<button onclick="TrackerApp.deleteVisionItem(' + index + ')" style="position: absolute; top: 5px; right: 5px; background: #ef4444; color: white; border: none; border-radius: 50%; width: 24px; height: 24px; cursor: pointer; font-size: 0.8rem;">✕</button>';
      container.appendChild(div);
    });
  }

  function addVisionItem() {
    const input = document.getElementById('visionItem');
    if (!input || !input.value.trim()) {
      alert('Please enter a vision item!');
      return;
    }
    
    appData.visionBoard.push(input.value.trim());
    input.value = '';
    saveData();
    renderVisionBoard();
  }

  function deleteVisionItem(index) {
    appData.visionBoard.splice(index, 1);
    saveData();
    renderVisionBoard();
  }

  // ===== STATS =====
  function updateStats() {
    var el = document.getElementById('totalDays');
    if (el) el.textContent = appData.stats.totalDays;
    
    el = document.getElementById('currentStreak');
    if (el) el.textContent = appData.stats.currentStreak;
    
    el = document.getElementById('goalsCompleted');
    if (el) el.textContent = appData.stats.goalsCompleted;
  }

  // ===== THEME =====
  function toggleTheme() {
    appData.theme = appData.theme === 'light' ? 'dark' : 'light';
    saveData();
    applyTheme();
  }

  function applyTheme() {
    if (appData.theme === 'dark') {
      document.body.classList.add('dark-mode');
    } else {
      document.body.classList.remove('dark-mode');
    }
  }

  // ===== DATA MANAGEMENT =====
  function exportData() {
    const dataStr = JSON.stringify(appData, null, 2);
    const dataBlob = new Blob([dataStr], { type: 'application/json' });
    const url = URL.createObjectURL(dataBlob);
    const link = document.createElement('a');
    link.href = url;
    link.download = 'top1percent-backup-' + new Date().toISOString().split('T')[0] + '.json';
    link.click();
    alert('Data exported successfully! 📥');
  }

  function importData() {
    const input = document.createElement('input');
    input.type = 'file';
    input.accept = 'application/json';
    input.onchange = function(e) {
      const file = e.target.files[0];
      const reader = new FileReader();
      reader.onload = function(event) {
        try {
          appData = JSON.parse(event.target.result);
          saveData();
          location.reload();
        } catch (error) {
          alert('Error importing data. Please check the file format.');
        }
      };
      reader.readAsText(file);
    };
    input.click();
  }

  function resetAllData() {
    if (confirm('⚠️ WARNING: This will delete ALL your data permanently. Are you absolutely sure?')) {
      if (confirm('This action cannot be undone. Confirm again to reset all data.')) {
        localStorage.removeItem('top1PercentData');
        location.reload();
      }
    }
  }

  // ===== DAILY RESET =====
  function checkDailyReset() {
    const today = new Date().toDateString();
    if (appData.stats.lastVisit !== today) {
      appData.habits.forEach(function(habit) {
        if (habit.completed) {
          habit.streak++;
        } else if (habit.streak > 0) {
          habit.streak = 0;
        }
        habit.completed = false;
      });
      
      appData.stats.totalDays++;
      appData.stats.lastVisit = today;
      saveData();
      renderHabits();
    }
  }

  // ===== INITIALIZATION =====
  function initApp() {
    loadData();
    loadDailyQuote();
    loadDailyAffirmation();
    renderHabits();
    renderGoals();
    renderJournal();
    renderGratitude();
    renderAffirmations();
    renderReflections();
    renderVisionBoard();
    updateStats();
    applyTheme();
    checkDailyReset();
  }

  // ===== GLOBAL API =====
  window.TrackerApp = {
    showSection: showSection,
    loadNewQuote: loadNewQuote,
    loadNewAffirmation: loadNewAffirmation,
    showRandomAffirmation: showRandomAffirmation,
    setMood: setMood,
    toggleHabit: toggleHabit,
    addCustomHabit: addCustomHabit,
    openCategoryPopup: openCategoryPopup,
    closeCategoryPopup: closeCategoryPopup,
    selectCategory: selectCategory,
    openGoalDetailsPopup: openGoalDetailsPopup,
    closeGoalDetailsPopup: closeGoalDetailsPopup,
    saveGoalFromPopup: saveGoalFromPopup,
    addGoal: addGoal,
    completeGoal: completeGoal,
    deleteGoal: deleteGoal,
    saveJournalEntry: saveJournalEntry,
    saveGratitude: saveGratitude,
    addCustomAffirmation: addCustomAffirmation,
    deleteAffirmation: deleteAffirmation,
    saveReflection: saveReflection,
    updateSlider: updateSlider,
    saveLifeWheel: saveLifeWheel,
    addVisionItem: addVisionItem,
    deleteVisionItem: deleteVisionItem,
    toggleTheme: toggleTheme,
    exportData: exportData,
    importData: importData,
    resetAllData: resetAllData
  };

  // ===== AUTO-INIT =====
  if (document.readyState === 'loading') {
    document.addEventListener('DOMContentLoaded', initApp);
  } else {
    initApp();
  }

})();
//]]>
</script>
