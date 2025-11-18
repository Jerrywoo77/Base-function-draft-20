# Base-function-draft-20
   function shareBase(uint256 _id, address _to) external {
        if (ownerOf(_id) != msg.sender) {
            revert NotYourBase(_id);
        }
        sharedBase[_to].push(_id);
    }
