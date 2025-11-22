# Loop-Variable
  Loop shareVariable(uint256 _id, address _to) external {
        if (ownerOf(_id) != msg.sender) {
            revert NotYourLoop(_id);
        }
        sharedLoop[_to].push(_id);
      }
