from flask import Flask, render_template
import random
app=Flask(__name__)
images=["http://img.buzzfeed.com/buzzfeed-static/static/2013-10/enhanced/webdr05/15/9/anigif_enhanced-buzz-26388-1381844103-11.gif"]
@app.route('/')
def index():
	url = random.choice(images)
	return render_template('index.html',url=url)
if __name__ == "__main__":
	app.run(host="0.0.0.0")
