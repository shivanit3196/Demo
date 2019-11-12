syntax = "proto2"

package practise;

option java_package = "com.practise";
option java_outer_classname = "TwitterMessageClass";

message IS_MAMMAL
{
    required bool is_domestic=1;
    optional bool is_wild=2;
}

message ANIMAL_INTERPRETATION
{
    required bool is_large_animal=1;
    required IS_MAMMAL is_mammal=2;
}

message TwitterMessage
{
    required double weight=1;
    optional string animal_type=2;
    required ANIMAL_INTERPRETATION animal_interpretation=3;
    optional double country=3;
}heloo