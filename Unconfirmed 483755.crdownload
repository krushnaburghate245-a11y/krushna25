import os
from flask import Flask

app = Flask(__name__)

@app.route("/")
def home():
    return "hello cloud"

# Fixed: Added double underscores to __name__ and "__main__"
if __name__ == "__main__":
    # It's good practice to use the environment variable for cloud deployments
    port = int(os.environ.get("PORT", 5000))
    app.run(host='0.0.0.0', port=port)