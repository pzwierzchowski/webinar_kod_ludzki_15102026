
How to run the project:
Requires Node.js 22, 24 or 26+.

1. clone the repo
2. navigate to repo location
3. install dependencies (_npm install_)
4. run cypress (_npx cypress open_) or run all tests headlessly (_npm test_)

## Selenium tests (Python)

Requires Python 3.10+, Google Chrome, and the Selenium dependencies:

1. Install dependencies: `python -m pip install -r requirements.txt`
2. Run the TS2 scenarios headlessly: `python -m pytest tests/test_ts2.py`

The tests use Selenium Manager to locate or download ChromeDriver. Set
`SHOP_BASE_URL` to override the default `https://tapsshop.pl/` URL.

Page interactions are grouped into page objects under `tests/page_objects/`;
the test scenarios themselves remain in `tests/test_ts2.py`.
