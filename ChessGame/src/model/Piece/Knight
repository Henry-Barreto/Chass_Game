@Override
public List getPossibleMoves() {
List moves = new ArrayList<>();
int[][] jumps = {
{-2, -1}, {-2, 1},
{-1, -2}, {-1, 2},
{1, -2}, {1, 2},
{2, -1}, {2, 1}
};
for (int[] jump : jumps) {
Position newPos = new Position(
position.getRow() + jump[0],
position.getColumn() + jump[1]
);
if (newPos.isValid()) {
Piece pieceAt = board.getPieceAt(newPos);
if (pieceAt == null || pieceAt.isWhite() != isWhite) {
moves.add(newPos);
}
}
}
return moves;
}