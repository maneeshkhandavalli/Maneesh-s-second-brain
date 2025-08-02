**Why it matters:**  
Let’s say someone tries to sign up using just “h” as their name and “123” as a password. That’s bad. Validation helps make sure the data users enter is:
- Correct
- Complete
### Where You Use It:
- Login & signup forms
- Contact forms
- Uploads
- Any kind of input basically
### What You Check:
- Is the email valid?
- Is the password long enough?
- Is the field empty?
- Are you getting what you expect? (text, number, date?)

### How You Do It in Backend (Node + Express):
- Use libraries like:
    - **express-validator** 🔗 [Docs](https://express-validator.github.io/docs/)
    - **Joi** 🔗 [Joi Docs](https://joi.dev/)