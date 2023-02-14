#include <iostream>
#include <sys/resource.h>
#include <unistd.h>

int main() {
  struct rusage usage;
  getrusage(RUSAGE_SELF, &usage);

  std::cout << "Maximum resident set size: " << usage.ru_maxrss << std::endl;
  std::cout << "Integral shared memory size: " << usage.ru_ixrss << std::endl;
  std::cout << "Integral unshared data size: " << usage.ru_idrss << std::endl;
  std::cout << "Integral unshared stack size: " << usage.ru_isrss << std::endl;
  std::cout << "Page reclaims: " << usage.ru_minflt << std::endl;
  std::cout << "Page faults: " << usage.ru_majflt << std::endl;
  std::cout << "Swaps: " << usage.ru_nswap << std::endl;
  std::cout << "Block input operations: " << usage.ru_inblock << std::endl;
  std::cout << "Block output operations: " << usage.ru_oublock << std::endl;
  std::cout << "Messages sent: " << usage.ru_msgsnd << std::endl;
  std::cout << "Messages received: " << usage.ru_msgrcv << std::endl;
  std::cout << "Signals received: " << usage.ru_nsignals << std::endl;
  std::cout << "Voluntary context switches: " << usage.ru_nvcsw << std::endl;
  std::cout << "Involuntary context switches: " << usage.ru_nivcsw << std::endl;

  return 0;
}
