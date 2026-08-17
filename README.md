# Coaching
1:1 coaching form
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Coaching Application</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&display=swap');
  
  * { margin: 0; padding: 0; box-sizing: border-box; }
  
  body {
    font-family: 'DM Sans', system-ui, sans-serif;
    background: #0a0a0a;
    color: #f5f5f5;
    min-height: 100vh;
    padding: 40px 20px;
    line-height: 1.5;
  }
  
  .container {
    max-width: 580px;
    margin: 0 auto;
  }
  
  .header {
    text-align: center;
    margin-bottom: 40px;
  }
  
  .header h1 {
    font-size: 28px;
    font-weight: 700;
    letter-spacing: -0.5px;
    margin-bottom: 8px;
  }
  
  .header .gold {
    color: #d4af37;
  }
  
  .header p {
    color: #999;
    font-size: 15px;
  }
  
  .card {
    background: #141414;
    border: 1px solid #222;
    border-radius: 16px;
    padding: 32px 28px;
  }
  
  .section-title {
    font-size: 13px;
    font-weight: 600;
    color: #d4af37;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-bottom: 20px;
    margin-top: 8px;
  }
  
  .field {
    margin-bottom: 20px;
  }
  
  label {
    display: block;
    font-size: 13.5px;
    font-weight: 500;
    color: #ccc;
    margin-bottom: 7px;
  }
  
  input, select, textarea {
    width: 100%;
    background: #0f0f0f;
    border: 1px solid #2a2a2a;
    border-radius: 10px;
    padding: 13px 14px;
    color: #fff;
    font-size: 15px;
    font-family: inherit;
    transition: border-color 0.2s;
  }
  
  input:focus, select:focus, textarea:focus {
    outline: none;
    border-color: #d4af37;
  }
  
  textarea {
    min-height: 100px;
    resize: vertical;
  }
  
  select {
    appearance: none;
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='12' fill='%23999' viewBox='0 0 16 16'%3E%3Cpath d='M8 11L3 6h10l-5 5z'/%3E%3C/svg%3E");
    background-repeat: no-repeat;
    background-position: right 14px center;
  }
  
  .row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 14px;
  }
  
  @media (max-width: 500px) {
    .row { grid-template-columns: 1fr; }
  }
  
  .submit-btn {
    width: 100%;
    background: #d4af37;
    color: #0a0a0a;
    border: none;
    border-radius: 12px;
    padding: 16px;
    font-size: 16px;
    font-weight: 700;
    font-family: inherit;
    cursor: pointer;
    margin-top: 12px;
    transition: background 0.2s, transform 0.1s;
  }
  
  .submit-btn:hover {
    background: #e0bd4a;
  }
  
  .submit-btn:active {
    transform: scale(0.98);
  }
  
  .note {
    text-align: center;
    color: #666;
    font-size: 12.5px;
    margin-top: 20px;
  }
  
  .divider {
    height: 1px;
    background: #222;
    margin: 28px 0;
  }
</style>
</head>
<body>
  <div class="container">
    <div class="header">
      <h1>Coaching <span class="gold">Application</span></h1>
      <p>Limited spots · $300/month</p>
    </div>
    
    <div class="card">
      <!-- 
        INSTRUCTIONS:
        1. Form is already set to send to dunedawes1@gmail.com
        2. Host this file anywhere (Carrd, your site, GitHub Pages, etc.)
        3. Or open it and test — FormSubmit will send results to your inbox
      -->
      <form action="https://formsubmit.co/dunedawes1@gmail.com" method="POST">
        
        <!-- FormSubmit settings -->
        <input type="hidden" name="_subject" value="New Coaching Application">
        <input type="hidden" name="_captcha" value="false">
        <input type="hidden" name="_template" value="table">
        <input type="hidden" name="_next" value="Coaching_ThankYou.html"> <!-- optional thank you page -->
        
        <div class="section-title">Personal Info</div>
        
        <div class="field">
          <label>Full Name *</label>
          <input type="text" name="name" required placeholder="Your name">
        </div>
        
        <div class="row">
          <div class="field">
            <label>Email *</label>
            <input type="email" name="email" required placeholder="you@email.com">
          </div>
          <div class="field">
            <label>Instagram / Handle</label>
            <input type="text" name="instagram" placeholder="@username">
          </div>
        </div>
        
        <div class="row">
          <div class="field">
            <label>Age *</label>
            <input type="number" name="age" required min="18" max="60" placeholder="25">
          </div>
          <div class="field">
            <label>Location</label>
            <input type="text" name="location" placeholder="City, Country">
          </div>
        </div>
        
        <div class="divider"></div>
        <div class="section-title">Current Stats</div>
        
        <div class="row">
          <div class="field">
            <label>Height</label>
            <input type="text" name="height" placeholder="5'11 or 180cm">
          </div>
          <div class="field">
            <label>Weight</label>
            <input type="text" name="weight" placeholder="180 lbs or 82kg">
          </div>
        </div>
        
        <div class="field">
          <label>Estimated Body Fat %</label>
          <select name="bodyfat">
            <option value="">Select range</option>
            <option>Under 10%</option>
            <option>10–12%</option>
            <option>13–15%</option>
            <option>16–18%</option>
            <option>19–22%</option>
            <option>23%+</option>
            <option>Not sure</option>
          </select>
        </div>
        
        <div class="field">
          <label>Training Experience *</label>
          <select name="experience" required>
            <option value="">Select</option>
            <option>Less than 1 year</option>
            <option>1–2 years</option>
            <option>3–5 years</option>
            <option>5+ years</option>
          </select>
        </div>
        
        <div class="divider"></div>
        <div class="section-title">Goals & Background</div>
        
        <div class="field">
          <label>Primary Goal *</label>
          <select name="primary_goal" required>
            <option value="">Select</option>
            <option>Build aesthetic physique (V-taper / shape)</option>
            <option>Get lean while keeping muscle + face</option>
            <option>Face + overall looksmaxxing</option>
            <option>Hormone optimization / performance</option>
            <option>Full transformation (body + face + presence)</option>
            <option>Other</option>
          </select>
        </div>
        
        <div class="field">
          <label>Current Hormone Situation</label>
          <select name="hormones">
            <option value="">Select</option>
            <option>Natural</option>
            <option>On TRT / Testosterone</option>
            <option>Using peptides</option>
            <option>Using anabolics / other compounds</option>
            <option>Previously used, currently off</option>
            <option>Prefer not to say</option>
          </select>
        </div>
        
        <div class="field">
          <label>What do you want to achieve in the next 90–180 days? *</label>
          <textarea name="goals_detail" required placeholder="Be specific..."></textarea>
        </div>
        
        <div class="field">
          <label>Biggest obstacle right now</label>
          <textarea name="obstacle" placeholder="Consistency, knowledge, recovery, hormones, etc."></textarea>
        </div>
        
        <div class="divider"></div>
        <div class="section-title">Commitment</div>
        
        <div class="field">
          <label>Coaching is $300 / month. Ready to start? *</label>
          <select name="ready" required>
            <option value="">Select</option>
            <option>Yes — ready to begin</option>
            <option>Yes — but I have a few questions first</option>
            <option>Interested, need more details</option>
            <option>Not right now</option>
          </select>
        </div>
        
        <div class="field">
          <label>Preferred start timeline</label>
          <select name="timeline">
            <option value="">Select</option>
            <option>Immediately</option>
            <option>Within 1–2 weeks</option>
            <option>This month</option>
            <option>Just exploring for now</option>
          </select>
        </div>
        
        <div class="field">
          <label>Anything else we should know?</label>
          <textarea name="extra" placeholder="Injuries, lifestyle, timeline, etc."></textarea>
        </div>
        
        <button type="submit" class="submit-btn">Submit Application</button>
        
        <p class="note">You’ll receive a response within 24–48 hours if selected.</p>
      </form>
    </div>
  </div>
</body>
</html>
