#ifndef GAME_H
#define GAME_H

#include "dork.h"

class Display{
private:
  string user_name;
  string level;
  int steps;
  int energy;
public:
  Display ();
  void info_display();
  void SetName();
  string GetName();
  string GetLevel();
  int GetEnergy();
  int GetSteps();
};

#endif
