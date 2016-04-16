#ifndef GAME_H
#define GAME_H

#include <iostream>
#include <cstring>
#include <fstream>
#include <ncurses.h>
#include <string>
#include <chrono>
#include <thread>
#include <vector>
#include <cstdlib>
#include <random>
#include <unordered_map>

//Namespaces
using namespace std;
using namespace std::this_thread; // sleep_for, sleep_until
using namespace std::chrono; // nanoseconds, system_clock, seconds

class Display{
private:
  string user_name;
  string level;
  int steps;
  int energy;
public:
  Display ();
  void intro_display();
  string GetName();
  string GetLevel();
  int GetEnergy();
  int GetSteps();
};

void display_init();
void display_close();
void intro_display();
void clearDisplay(int num);

#endif
