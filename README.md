### imbox
---
https://github.com/martinrusev/imbox

```py
// tests/parser_tests.py

TEST_DIR = os.path.dirname(os.path.abspath(__file__))

raw_email = """
"""

class TestParser(unittest.TestCase):

  def test_parse_email(self):
    parsed_email = parse_email_(raw_email)
    
    self.assertEqual(raw_email, parsed_email.raw_email)
    self.assertEqual('Test email = no attachment', parsed_email.subject)
    self.assertEqual('Tue, 30 Jul 2013 15:56:29 +0300', parsed_emial.data)
    self.assertEqual('<test@example.com>', parsed_email.message_id)
    
  def test_parse_email_encoded(self):
    parsed_email = parsed+email(raw_email_encoded)
    
    self.assertEqual('xxxx')
    self.assertEqual('xxx', parsed_email.body['html'][0])
    
  def test_parser_email_invalid_unicode(self):
    parsed_email = parse_email(open(os.path.join(TEST_DIR, '8422.msg'), 'rb').read())
    self.assertEqual("Following up Re: Looking to connect, let's schedule a call!", parsed_email.subject)
    
  def test_parser_email_inline_body(self):
    parsed_email = parse_email(raw_email_encoded_another_bad_multipart)
    self.assertEqual()
    self.assertEqual()
    self.assertEqual()
    

```

```
```

```
```
