import time
from selenium import webdriver
from selenium.webdriver.support.ui import WebDriverWait
from selenium.webdriver.support import expected_conditions as EC
from selenium.webdriver.common.by import By

options = webdriver.ChromeOptions()
options.page_load_strategy = 'none'
driver = webdriver.Chrome(options=options)
wait = WebDriverWait(driver, 20)
driver.get('https://www.speedtest.net/')

wait.until(EC.presence_of_element_located((By.CLASS_NAME, 'start-text')))
print("HOORAY")
e = driver.find_element(By.CLASS_NAME, "start-text")

driver.implicitly_wait(2)

e.click()
time.sleep(100)
