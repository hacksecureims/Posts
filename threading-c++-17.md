# Threading C++ 17

Implémentation des threads dits "modernes" dans une classe. Le programme écrira 5 fois "message".

```
#include <functional>
#include <thread>
#include <mutex>
#include <iostream>

class Test {
private:
  std::shared_ptr<std::thread> th;
  std::atomic<bool> thread_stop = false;
  
  void run(){
    while(!thread_stop){
	  std::cout << "message" << std::endl;
      std::this_thread::sleep_for(std::chrono::seconds(1));
    }
  };
  
public:
  void start(){
    th = std::make_shared<std::thread>([this] () {this->run(); });
  };
  
  void stop(){
    thread_stop = true;
    th->join();
  };
};

int main(int argc, char* argv[]){
  Test t;
  t.start();
  std::this_thread::sleep_for(std::chrono::seconds(5));
  t.stop();
  return 0;
}

```
