import webapp2
class MainPage(webapp2.RequestHandler):
    def get(self):
        self.response.write("Rohan Loves Sejal")

app=webapp2.WSGIApplication([('/',MainPage)], debug=True)

runtime: python27
api_version: 1
threadsafe: false

handlers:
  - url: /
    script: test.app
