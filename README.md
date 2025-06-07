  SauceDemo QA Assessment

   Notes

  Prerequisites
- Python 3.8 or later
- Google Chrome browser installed
- ChromeDriver installed and added to PATH
- Install required Python packages:
  ```bash
  pip install -r requirements.txt•	Postman installed (for API testing)
	•	Git installed for version control
	•	Stable internet connection (site is hosted online)

  
Observations
	•	problem_user shows broken product images on the Products page.
	•	Cart badge sometimes updates slowly when quickly adding/removing items.
	•	Login error messages are small and lack strong visual feedback.
	•	“Reset App State” option provides no visible confirmation or redirect.
	•	Checkout confirmation page lacks detailed order info or next steps.

 Blockers
	•	No visible API for products/cart endpoints (only /users tested).
	•	UI inconsistencies with problem_user affected automation stability.
	•	No API token or login session exposed for token-based validation.
	•	Minimal feedback for reset action made state-tracking harder.


Bug Report & Suggestions

Full details are available in the attached PDF (reports/test_case_report.pdf), but key bugs include:
	•	BUG01: Broken product images for problem_user
	•	BUG02: Cart badge update delay
	•	BUG03: Weak feedback on failed login
	•	BUG04: No confirmation after resetting app state


Suggested improvements:
	•	Use fallback images
	•	Stronger error validation
	•	Add loading spinners during filter
	•	Improve checkout form validation
	•	Add screen reader support (accessibility)


Tools Used
	•	Selenium WebDriver (Python)
	•	Postman (API testing)
	•	Manual testing
	•	Bug reporting
	•	PDF for test case documentation


