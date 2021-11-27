[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)


# Test Internet Connection Speed Using Python


## Running Script

To run Script, run the following command

```bash
  Python Main.py
```


### Installation
install the required library into our computer. Just run this code in your terminal or command line.

```
  pip install speedtest-cli
```
 ## Script   

```
import speedtest
speed = speedtest.Speedtest()
```

```
def main():
    while True:
        print('\a')
        choice=int(input("""Check Your Connection Speed
    1) Download Speed
    2) Upload Speed
    3) Exit
Choice (1/2/3): """))
        print('\a')
...
if __name__ == '__main__':
  main()
  ```

```
if choice==1:
            print('Counting...')
            print(f"Download speed: {'{:.2f}'.format(speed.download()/1024/1024)} Mb/s")
        elif choice==2:
            print('Counting...')
            print(f"Upload speed: {'{:.2f}'.format(speed.upload()/1024/1024)} Mb/s")
        elif choice==3:
            print('Exiting the program')
            quit()
        else:
            print("Please choose the correct options")
```


