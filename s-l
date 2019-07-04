#!/bin/bash
# script to expand short url
if [ -n "$1" ]; then 
	if [[ $1 =~ https://* ]]; then
	echo "
Short url :
$1	"
LONG=$(curl -sI "$1" | grep ^location | cut --delimiter=" " -f 2)
	echo "
Long url :
$LONG "
	else
		echo "not a url" >&2
	fi
fi
if [ -z "$1" ]; then
	echo "Enter url"
fi
